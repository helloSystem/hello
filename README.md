# hello  [![](https://img.shields.io/badge/dynamic/json?color=orange&label=DistroWatch&query=popularity&url=https%3A%2F%2Fdiwa.demo-web-fahmi.my.id%2Fapi%2Fv2%2Fdistributions%2FhelloSystem)](https://distrowatch.com/hellosystem)

![](https://github.com/helloSystem/hello/blob/master/branding/computer-hello.png?raw=true)

### Please see https://hellosystem.github.io/ for documentation.

This repository is where developers and interested advanced users brainstorm on __helloSystem__. If you are looking for documentation, Live ISO downloads, and other _practical_ information, look at https://hellosystem.github.io/.

## Screenshot

![Screenshot](https://github.com/helloSystem/hello/blob/master/screenshots/20211219-desktop-0.7.png)

## What?

A desktop system for creators that focuses on simplicity, elegance, and usability.

Following the published [Human Interface Guidelines](https://dl.acm.org/doi/book/10.5555/573097), and [First Principles of Interaction Design](https://asktog.com/atc/principles-of-interaction-design/) liberally re-interpreted for today.

[Based on FreeBSD](https://en.wikipedia.org/wiki/MacOS#/media/File:Unix_timeline.en.svg).

For mere mortals. Welcoming to switchers from macOS.  Not just a theme. Not a clone of anything, but something with which the long-time Mac user should feel instantly comfortable. The latest technologies, without the complexities of Linux distributions. Without lockdown. Without Big Brother. The user in full control.

Less, but better!

## Why?

Because we used to like the Mac, since 1984.

* Consistent user interface across all applications (e.g., all applications have the same global menu bar, and all applications have File -> Quit in them with the same Command-Q shortcut)
* Consistent user interface over time (e.g., the above has not changed since 1984)
* WYSIWYG: Black text on white background, like on paper. Not amber on black or green on black like  most computers before it
* No need to use the command line
* No confusing text messages when the system is starting
* Everything done via the global menu bar
* Menu shortcuts on the Command key (the key left to the spacebar)
* Easy to use disk images
* Spatial file manager (e.g. every document or folder has one, and exactly one place on the screen; each window and each object inside a window keeps its location on screen)
* Applications can be "managed" by drag and drop in the file manager
* Every application is one file (or one "bundle", which is one object in the file manager)
* No complicated text commands to learn, no need to use a Terminal application

Because we used to like the Mac, since 1984. But it's increasingly getting... difficult:

* Because according to Edward Snowden, [Apple Just Declared War on Your Privacy](https://edwardsnowden.substack.com/p/all-seeing-i) (all the while talking about "privacy", "security", "trusted")
* Because Apple has become Big Brother by even considering [Client-Side Scanning](https://arxiv.org/abs/2110.07450), distrusting its users and treating them like potential criminals, searching through users' data
* Because Apple runs services like [Visual Lookup](https://eclecticlight.co/2022/03/25/how-visual-look-up-works-in-detail-2-object-recognition-and-live-text)and `mediaanalysisd` on macOS which may leak data from the local system to the OS vendor's servers (and potentially anyone surveilling them)
* Because Apple thinks that ["Sideloading is a cyber criminal’s best friend"]( https://twitter.com/verge/status/1455983636830990337) - and wants to be the gatekeeper for everything that runs on _your_ device
* Because App Stores allow governments to prevent certain applications from being used https://www.washingtonpost.com/world/2022/03/12/russia-putin-google-apple-navalny/
* Because we want "Personal Digital Sovereignty", in other words: be in full control over what our devices are doing
* Because Apple has become ["anti-hacking"](https://twitter.com/jeremy_soller/status/1448318637488566273)
* Because we want to run apps from "unidentified developers" that need no blessing by the operating system vendor and no workarounds like https://lapcatsoftware.com/articles/textedit-gatekeeper.html (Note: Maybe `sudo spctl --master-disable` does the trick if you are root on the machine, which means no luck on "managed" devices)
* [Gatekeeper](https://en.wikipedia.org/wiki/Gatekeeper_(macOS)) ("It forced Mac developers, who had previously been legally free, to sign a strict contract." [Source](https://twitter.com/lapcatsoftware/status/1440735016611246086)) (Note: Maybe `sudo spctl --master-disable` does the trick if you are root on the machine, which means no luck on "managed" devices)
* @antranigv on *macOS to FreeBSD migration a.k.a why I left macOS* https://antranigv.am/weblog_en/posts/macos_to_freebsd/
* https://hardware.substack.com/p/falling-out-of-love-with-apple-part1
* https://medium.com/@probonopd/bring-back-the-ease-of-80s-and-90s-personal-computing-393738c5e2a1 (Medium article written by me)
* https://memoryprotection.show/blog/episode-24 ("It has become very user-hostile.")
* Because what used to be simple is becoming increasingly difficult. Example: Install a kernel extension https://twitter.com/CastIrony/status/1444077820041318400 - probably the process doesn't even work on "managed" devices where some central IT department thinks it knows best which kexts the users "need". Lock in and lock down
* https://bombich.com/blog/2021/05/19/beyond-bootable-backups-adapting-recovery-strategies-evolving-platform (If the soldered-in SSD fails, you cannot boot from external bootable media, because "security")
* Because we want all software to be "sideloaded" rather than coming from monopolistic stores https://www.lunduke.com/2021/07/google-goes-to-war-against-sideloading/
* Because we disagree with phone-home, tracking, activation. Apparently it is not necesseary to [activate](https://twitter.com/EggFreckles/status/1439621327472762888) Macs. Has the NSA ordered this "feature" so that they can track people even better?
* Because Apple is spying on you. Yes. Despite all the talk about "privacy" there is the [DSID](https://proton.me/blog/apple-ad-company)
* Because used Apple devices have to be thrown away if they are "FMIP locked" (which regularly happens with previously company-owned devices) https://twitter.com/TWArecycles/status/1444549353335509003
* Because all the locks and shackles Apple is putting on their devices is filling nothing but the landfills and their pockets https://twitter.com/RDKLInc/status/1477410245131616256
* Because Apple user interfaces are becoming less and less Mac-like (as measured by the original Human Interface Guidelines). Example: [The Tragedy of Safari 15 for Mac’s ‘Tabs’](https://twitter.com/daringfireball/status/1444092268344840197)
* Because Mac OS X has been deteriorating ever since the "Back to the Mac" event in 2010 https://512pixels.net/2014/04/aqua-past-future/, becoming less like the Mac and more like iOS
* Because the user experience has been getting worse and worse, and here is why https://www.fastcompany.com/3053406/how-apple-is-giving-design-a-bad-name
* Because Apple is watering the desktop down with inferior mobile UX and hybrid apps ("Catalyst") that don't behave like real mouse-centric ("AppKit") desktop apps
* [Louis Rossmann: A reminder of how computing used to be](https://www.youtube.com/watch?v=JdHjflBiSMI)

Lock-down:

* https://sneak.berlin/20201112/your-computer-isnt-yours/
* https://sneak.berlin/20201204/on-trusting-macintosh-hardware/

Irrepairable, non-upgradeable hardware: 

* https://www.macrumors.com/2018/10/04/t2-macs-must-pass-diagnostics-for-certain-repairs/
* https://www.vice.com/en/article/yw9qk7/macbook-pro-software-locks-prevent-independent-repair
* https://uk.pcmag.com/old-news/117795/apples-t2-chip-makes-third-party-mac-repairs-impossible

Less and less Mac-like desktop user experience:

* [Riccardo Mori: The reshaped Mac experience](http://morrick.me/archives/9150)
* [Riccardo Mori: A retrospective look at Mac OS X Snow Leopard](http://morrick.me/archives/9220)
* [Riccardo Mori: A retrospective look at Mac OS X Snow Leopard - Addendum](http://morrick.me/archives/9246)

## How?

Just follow Bruce Tognazzini's [First Principles of Interaction Design](https://asktog.com/atc/principles-of-interaction-design/)

https://asktog.com/atc/principles-of-interaction-design/

## Contributing

__This project lives from *your* involvement.__

Please see https://hellosystem.github.io/docs/developer/contributing

We need help with [issues flagged with help-wanted](https://github.com/search?q=org%3AhelloSystem+is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) – maybe you'd like to look into [issues flagged with good-first-issue](https://github.com/search?q=org%3AhelloSystem+is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22&type=). Other contributions are, of course, welcome.

### Links

* [helloSystem Documentation](https://hellosystem.github.io/docs/)
* https://github.com/probonopd/hello/wiki
* [High-level architecture](../../wiki/Architecture)
* [Brainstorming](../../wiki/Brainstorming)
* [Welcome and unwelcome technologies](../../wiki/Welcome-and-unwelcome-technologies)
* [Make. It. Simple. Linux Desktop Usability – parts 1–6](https://www.reddit.com/r/linux/comments/enp56v/make_it_simple_linux_desktop_usability_part_1/) – user experience (UX) discussion on Reddit (January 2020, archived)
