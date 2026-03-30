# Setting Up a Development Environment for RotU

**Applies to:** RotU 2.2  
**Tested on:** Microsoft Windows Vista, Microsoft Windows 7  
**Status:** Final

## Introduction

This page contains instructions and information about setting up a development environment for **Reign of the Undead (RotU)**.

## Prerequisite Software

All of the software below is either [Free Software](http://www.gnu.org/licenses/gpl.html) or [Open Source Software](http://opensource.org/), except for the **COD Mod Tools**, which is governed by Activision/IW's EULA. All software is available at no cost.

### Subversion
You need a Subversion client to download the source code.  
**Recommended:** [TortoiseSVN](http://tortoisesvn.net/)  
[TortoiseSVN Primer](http://tortoisesvn.net/docs/release/TortoiseSVN_en/tsvn-dug.html)

### Perl
The build system is written in Perl.  
**Recommended:** [Strawberry Perl](http://strawberryperl.com/)

### Text Editor
A good programmer's text editor is required.  
**Strongly recommended:** [Kate (KDE Advanced Text Editor)](http://kate-editor.org/get-it/)

> Note: Notepad is **not** sufficient. Wordpad is not a real text editor.

### Kompare
Useful for viewing unified diff files (`.diff`).  
Usually installed together with the KDE for Windows tools (when you install Kate).

### GIMP
For editing raster images (textures, etc.).  
**Recommended:** [GIMP](http://www.gimp.org/) + [GIMP DDS Plugin](http://code.google.com/p/gimp-dds/)

### Inkscape
For editing SVG (Scalable Vector Graphics) files.  
**Recommended:** [Inkscape](http://inkscape.org/)

### COD4 Mod Tools
Required to build the mod.  
Download: [Call of Duty 4 Modern Warfare Mod Tools](http://callofduty.filefront.com/file/Call_of_Duty_4_Modern_Warfare_Mod_Tools;85947)

## Backup CoD4

Before you begin, **strongly recommended**:  
Zip your entire `CoD4` folder and store it somewhere safe in case anything goes wrong.

## Get the Source Code

Use your Subversion client to check out the source code to a convenient local working directory.

> **Important**: Do **not** put the working copy inside your CoD4 folder.  
> Example location: `C:\Users\Mark\work\rotu\trunk`

### Anonymous Checkout (recommended for most users)
```plaintext
http://reign-of-the-undead.googlecode.com/svn/trunk
```

### Developers Checkout

  Developers should checkout using a secure https connection using the credentials you were given:

```plaintext
https://reign-of-the-undead.googlecode.com/svn/trunk
```

## Configure the Build System
The build system is contained primarily within `build\makeMod.pl`.  The configuration for `makeMod.pl` is contained in `build\makeConfig.pl`. Using your text editor, open `makeConfig.pl` and edit the `codPath`, `modPath`, and `uploadPath` variables as required for your system. Save your changes, then use your text editor to open `makeMod.pl`.

The first line is the path to the perl interpreter you previously installed. You need to edit the line as required, depending on where you installed perl.  Make sure the line begins with the shebang `#!`, and that it is the very first line in the file.  Save your changes, then close the files.

### Windows 7 Note:
If your `CoD4` install is on a different drive than the source code you downloaded, the mod will not compile as is.  This is because Microsoft changed the 'cd' command.  If this applies to you, delete the file `build\makeFF.bat`, then rename `build\makeFF_win7.bat` to `build\makeFF.bat`.

## Configure the the Mod
In the src folder are several `*_default.cfg` configuration files.  These files will need to be edited. Using your text editor, open each of these files and save it in the src folder without the `_default`, i.e. save `server_default.cfg` as `server.cfg`.  *After* you have saved the file under the new name, edit the config settings as appropriate for your system and as desired.

In the src folder are several `*_default.bat` batch files.  These files will need to be edited. Using your text editor, open each of these files and save it in the src folder without the `_default`, i.e. save `playMod_default.bat` as `playMod.bat`.  *After* you have saved the file under the new name, edit the batch file as appropriate for your system and as desired.

## Build the Mod
To build the mod, open a command line (cmd.exe, i.e. 'Command Prompt'), then cd as required to get to the build directory (C:\Users\Mark\work\rotu\trunk\build or similar). To get an idea of makeMod.pl's features, at the command prompt execute

`perl makeMod.pl -h`

Once you've read that brief documentation, execute

`perl makeMod.pl`

to build the mod.  Building may take a minute or more, depending on the speed of your computer.  When the script finishes, the mod will have been compiled, installed, and relevant files copied to the uploadPath you specified in `makeConfig.pl`.

## Play the Mod
Using your file manager, browse to the modPath you specified earlier, then click on `playMod.bat` to play the mod.  If it starts up OK, it is safe to copy the files from the uploadPath to your server.

**New home of the source code**: [https://github.com/marktaff/reign-of-the-undead](https://github.com/marktaff/reign-of-the-undead)

*Originally released from the Google Code SVN repository.*
