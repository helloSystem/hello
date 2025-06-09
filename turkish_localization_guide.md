# Enabling Turkish Language Support in helloSystem

This document outlines the process for enabling Turkish language support in helloSystem, based on investigations of the system's documentation and localization infrastructure.

## 1. Availability of Translations

*   **Confirmation:** Turkish translations for helloSystem components are **100% complete** on the Weblate platform.
*   **Weblate Project Link:** You can view the helloSystem translation project, including Turkish, on Weblate: [https://hosted.weblate.org/projects/hellosystem/](https://hosted.weblate.org/projects/hellosystem/)
*   **Download Translations ZIP:** A ZIP file containing all available translation files (including Turkish `.ts` files) can be downloaded directly from: [https://hosted.weblate.org/download/hellosystem/?format=zip](https://hosted.weblate.org/download/hellosystem/?format=zip)

## 2. Localization Mechanism

helloSystem employs Qt-based localization technologies for its applications:

*   **`.ts` Files (Translation Source):** These XML-based files contain the source text and its translations.
    *   **Python Applications:** Python applications in helloSystem (typically using PyQt) utilize `.ts` files directly at runtime. A custom script, `tstranslator.py`, is often used to load these translations without a separate compilation step for the translations themselves.
    *   **Qt (C++) Applications:** These applications also use `.ts` files as the source for translations.
*   **`.qm` Files (Qt Message):** For Qt (C++) applications, the `.ts` files are compiled into compact binary `.qm` files using Qt's `lrelease` tool. These `.qm` files are then loaded by the applications at runtime.

## 3. Integration Steps (Conceptual)

For Turkish translations to be active in the system, the appropriate translation files must be correctly placed within each application's bundle or system resource directories. This is typically handled during the system image build process or via language pack installation.

*   **For Python Applications:**
    *   Extract the downloaded translations ZIP file from Weblate.
    *   Locate the Turkish translation file for the specific Python application or component (e.g., `Utilities/tr.ts` if the application is part of the "Utilities" component).
    *   Place this `tr.ts` file into the application's designated internationalization directory. The standard path is usually `AppName.app/Contents/Resources/i18n/tr.ts`.

*   **For Qt (C++) Applications:**
    *   The Turkish `.ts` file (e.g., `Filer/tr.ts` for the Filer application) needs to be compiled into a `tr.qm` file using `lrelease`.
    *   This `tr.qm` file must then be installed into the location where the application expects to find its translation files (e.g., often a `translations` or `i18n` subdirectory within the application's resources, such as `Filer.app/Contents/Resources/translations/tr.qm`). This step is typically integrated into the application's build system.
    *   If the Weblate ZIP download directly provides `.qm` files, those could potentially be used, but compiling from `.ts` is the standard approach.

## 4. Language Selection by User

Once the Turkish translation files are integrated into the system:

*   **Keyboard Preferences Application:** The user can select their preferred language through the "Keyboard preferences application". This application allows users to choose their "keyboard layout (language)".
*   **System Locale Setting:** Selecting "Turkish" in this application is expected to:
    1.  Change the active keyboard layout to Turkish.
    2.  Set the system-wide locale to Turkish (e.g., by setting environment variables like `LANG=tr_TR.UTF-8`). This allows applications that support localization to detect the user's preference and load the corresponding Turkish translation files (`.ts` or `.qm`), displaying their user interface in Turkish.
*   This aligns with helloSystem's automatic language detection features (via EFI variables or Raspberry Pi keyboards), which also point to a system-wide language setting.

## 5. Note on Current Investigation Limitations

The information in this guide is based on documentation review and examination of the project's online resources. Direct file system manipulation, ZIP file extraction, and modification of a live helloSystem environment were not possible with the toolset used for this investigation. Therefore, this document serves as a guide for manual integration by developers, system builders, or users comfortable with system modifications, or for configuring the helloSystem build process to include Turkish localization by default.

---
For further details on specific applications or build processes, refer to the helloSystem developer documentation and the respective application repositories.
