# OmniAutomation

This repository contains a collection of scripts that I use to
automate OmniGroup applications. Currently, these focus on OmniFocus,
as I use it daily.

## Focus

Initially, this repository will convert the suite of AppleScript-based
OmniFocus scripts that I use daily to OmniAutomation (Javascript) and
provide compatibility with OmniFocus 4.

## Installation

`tl;dr`: Copy the contents of the `PlugIns/` directory from this
repository to a folder on your iCloud Drive and then use [Add Linked
folder…](https://omni-automation.com/plugins/linked-folders.html) in
each of your Omni Applications to add that folder as a plug-in source.

The latest suite of Omni applications include a new plug-in management
architecture that enables you to designate both local and remote
directories as sources for Omni Automation plug-ins. See the “Linked”
Folders
[Documentation](https://omni-automation.com/plugins/linked-folders.html)
on the [Omni Automation](https://omni-automation.com/) site.

The [Omni Automation](https://omni-automation.com/) site also provides
detailed information for:

- [Omni Automation: Plug-In Installation on
  iOS](https://omni-automation.com/plugins/installation-iOS.html)
- [Omni Automation Plug-Ins: Installation on
  iPadOS](https://omni-automation.com/plugins/installation-iPadOS.html)
- [Omni Automation: Shared iCloud Plug-In Folder on
  iPadOS](https://omni-automation.com/plugins/installation-iPadOS-iCloud.html)

### Sample Installation

Assuming you have created `OmniAutomation-Plug-Ins` in your iCloud
Drive, the follow will copy the plugins to that directory. Note the
trailing `/` on the source so that you copy the *contents* of
`Plug-Ins`, not the directory.

```sh
$ pwd
/Users/XXX/OmniAutomation

$ rsync --verbose --checksum --archive --delete --delete-excluded ./Plug-Ins/ ~/Library/Mobile\ Documents/com\~apple\~CloudDocs/OmniAutomation-Plug-Ins
```

## Inspiration

My daily AppleScripts come from a variety of sources, including:

- [curtclifton/OmniFocusScripts: Various scripts for automating
  OmniFocus](https://github.com/curtclifton/OmniFocusScripts)
- [lemonmade/templates: Templates Applescript for
  OmniFocus.](https://github.com/lemonmade/templates)
- [dbyler/omnifocus-scripts: Scripts for use with
  OmniFocus](https://github.com/dbyler/omnifocus-scripts)
- [brandonpittman/OmniFocus: Scripts for
  OmniFocus](https://github.com/brandonpittman/OmniFocus)
