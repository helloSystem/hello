# Contributing

If you have found this page, chances are that you are considering to to contribute to this project.

Awesome!

This is a small, purely volunteer-driven project, so your contributions are _highly_ welcome.

## How to get started?

* Download the pre-alpha Live ISO from https://github.com/helloSystem/ISO/releases/tag/continuous-hello
* Look through the GitHub Issues sections of the projects within https://github.com/helloSystem/
* A great way to get started is to comment on some GitHub issues. Also feel free to open new ones. We use GitHub Issues as a means of discussion and keeping track of everything, so don't hesitate to use them. General topics not related to any particular component go to https://github.com/helloSystem/hello/issues
* Especially have a look at issues marked with ![](https://user-images.githubusercontent.com/2480569/97901371-64b8ad80-1d3c-11eb-8282-0bfdcd3fe512.png). Here your contributions would be especially helpful, but of course your contibutions to other tickets are more than welcome, too
* There is a liberal amount of `FIXME` and `TODO` in the source code. Reducing the number of those is always highly welcome

## Our project values

* Please see https://github.com/helloSystem/hello for the general philosophy of the project
* Always keep in mind that our philosophy is "simple > complicated", "less, but better"
* We prefer small pull requests that change one thing each, rather than large ones that do many things at once
* Please avoid complex code structures that require deep C++ knowledge (e.g., avoid subclassing, pointer arithmetic,... where possible)
* We appreciate code with comments that explain why we are doing something
* Our policy is to merge PRs liberally but roll back changes that cause breakage quickly. `master` must always build and not crash

## Areas we especially need help with

Here is what we need help with: [Issues flagged with help-wanted](https://github.com/search?q=org%3AhelloSystem+is%3Aissue+is%3Aopen+label%3A%22help+wanted%22), and of course other contributions are also welcome.

Maybe you'd like to look into one of these: [Issues flagged with good-first-issue](https://github.com/search?q=org%3AhelloSystem+is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22&type=).

### FreeBSD related topics

Skills/resources we don't currently have and would highly appreciate help with

|Skillset needed|Topic|Status|Rationale|Contact|
|---|---|---|---|---|
|FreeBSD kernel|Overhaul/bugfixing for unionfs.ko to remove crashes in FreeBSD 13 when attempting to create a read-write root filesystem|Idea|Improve robustness of the Live system infrastructure|probonopd|
|OpenZFS|A way to combine read-only (Live ISO) with read-write (ramdisk) to create a read-write root filesystem|Idea|Use ZFS for the Live system without the need for unionfs|probonopd|
|FreeBSD kernel, graphics|Zero-text bootsplash that shows a boot animation and hides all text unless verbosity is explicitly requested|Idea|Put together "appliance" style systems that are not frightening non-technical users|probonopd|
|FreeBSD build system|Kernel-related packages built for each FreeBSD version ([details](https://github.com/furybsd/furybsd-livecd/issues/241))|idea|Xorg fails on 12.2-RELEASE|probonopd|
|FreeBSD Linuxulator|Make it possible for Linux applications to use FreeBSD D-Bus|Idea|Have Linux applications to use the [global menu](https://github.com/helloSystem/Menu) that is running on FreeBSD|probonopd|
|FreeBSD kernel, Golang|Enable Go-based FUSE filesystems for FreeBSD ([issue](https://github.com/jacobsa/fuse/issues/91))|Idea|Packages that are images rather than archives: Experiment with [distr1](http://distr1.org/) concepts on FreeBSD|probonopd|
|Qt, OpenZFS|ZFS snapshot, clone integration into the file manager|Idea|Expose the power of ZFS to non-technical users|probonopd|

### Qt related topics

|Skillset needed|Topic|Status|Rationale|Contact|
|---|---|---|---|---|
|Qt|Improve the Filer (file manager)||Please see https://github.com/helloSystem/Filer/issues|probonopd|
|Qt|Improve the Menu (global menu bar)||Please see https://github.com/helloSystem/Menu/issues|probonopd|
