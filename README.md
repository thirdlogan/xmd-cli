# xmd-cli
Yes, please! Moar metadata. A set of cli utils and automation workflows (for MacOS and Linux).

The bash/zsh cli tools are:
> * getxmd
> * setxmd
> * addxmd
> * rmxmd

The automation workflows for MacOS are custom actions for the Finder via [Automator](https://developer.apple.com/documentation/automator), and the automation scripts for Linux are custom actions for the file browser [Thunar](https://github.com/xfce-mirror/thunar) via [Thunar Custom Actions](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwjokqTL-c_pAhXDX80KHSUmCEAQFjADegQIBRAB&url=https%3A%2F%2Fhelp.ubuntu.com%2Fcommunity%2FThunarCustomActions&usg=AOvVaw3lmkEFBiiL3HGDgpi_FRGR).  

## MacOS

### Installing MacOS Dependencies
This has dependencies on `exiftool` and `tag`, both available through [homebrew](https://formulae.brew.sh/). Install `homebrew`, then execute the command:
> `brew install exiftool tag`

### Installing MacOS cli tools
Just copy the four scripts from this repo's `macos` directory somewhere that is in your `$PATH`.

### Installing Automator workflows
Copy `Xmd - Get.workflow` and `Xmd - Set.workflow` to either `/Library/Automator` for use by all users, or `~/Library/Automator` for just your user.


## Linux

### Installing Linux Dependencies
This has dependencies on `exiftool` and `tag`, both of which should be available via your distro's package manager. I mostly use Ubuntu, so for me the command is 
> `sudo apt install exiftool tag`

### Installing Linux cli tools
Just copy the four scripts from this repo's `linux` directory to somewhere that is in your `$PATH`.

### Installing the Thunar workflows
These are just simple scripts added to the `User Custom Actions` that can be accessed from the drop-down `Edit` menu. Just add them to `thunar-setxmd` and `thunar-getxmd` as whatever you would like to call them.

## Copying, redistributing, etc.
These are 100% free! Fork this repo, rip-off these little scripts, do whatever you'd like. If you get some use out of them, you're making me smile. 