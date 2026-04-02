
# Kubuntu 25.10 CoD4 Install Notes
Installed 31 March 2026

## Install Wine

```
apt install wine
```

## Get the Game
If you have the DVD, and your machine has a DVD drive, you can install normally. If your machine doesn't have a DVD drive, you will need to rip the DVD to an *.iso file.  If you want to play the game without having the DVD in the drive, you will need a patched copy of `iw3sp.exe`. You can find such patched copies on the Internet.

## Get Product Key

The product key should be in/on the DVD case.  Otherwise, you can find them on the Internet. They are shaped like the two invalid keys below:

```
EY3M-RWU1-7C06-MVZG-B9AD   <-- Invalid
Q6EA-31EB-4J73-T8K0-D838   <-- Invalid
```

## Mount ISO & Install CoD4

```
sudo mkdir -p /mnt/iso
sudo mount -o loop "/home/mark/cod4/Call of Duty 4 - Modern Warfare.iso" /mnt/iso

# Run installer
cd /mnt/iso
wine setup.exe
```

This installs CoD4 1.0.255.  Need to upgrade to 1.7.

The version 1.0.255 corresponds to the original, unpatched release of Call of Duty 4: Modern Warfare (often referred to as 1.0). Users on this version frequently encounter issues accessing modern multiplayer servers, which typically require the 1.6 or 1.7 patches for compatibility.

Patching to 1.7 is **REQUIRED**

## Patching to Version 1.7

To resolve connectivity issues and access the full multiplayer experience, players must install the 1.7 patch, which updates the version.inf file to ExtVersion=1.7 and IntVersion=28.2.  This update is essential for connecting to active community servers and utilizing the latest game features available on platforms like COD4x and Promod.

After patching, the game's `version.inf` file should display ExtVersion=1.7 to confirm the update.
N.B. `version.inf` won't exist until after you patch the base game the first time.

A *.rar file containing all the [patches](https://www.moddb.com/games/call-of-duty-4-modern-warfare/downloads/call-of-duty-4-modern-warfare-all-patches) from 1.1 through 1.7 is available from ModDB.

```
# Run each command sequentially. When the installer finishes, run the next one.
# Don't Panic.  Some patches are very quick, some take significantly longer.
wine "/home/mark/cod4/CoD4.patches/CoD4MW - 1.1.exe"
wine "/home/mark/cod4/CoD4.patches/CoD4MW - 1.2.exe"
wine "/home/mark/cod4/CoD4.patches/CoD4MW - 1.3.exe"
wine "/home/mark/cod4/CoD4.patches/CoD4MW - 1.4.exe"
wine "/home/mark/cod4/CoD4.patches/CoD4MW - 1.5.exe"
wine "/home/mark/cod4/CoD4.patches/CoD4MW - 1.6.exe"
wine "/home/mark/cod4/CoD4.patches/CoD4MW - 1.7.exe"
```

## Backup CoD4 Again

After patching to 1.7, **strongly recommended**:  
Zip your entire `CoD4` folder and store it somewhere safe in case anything goes wrong, e.g. `CoD4.patched.to.1.7.zip`

## Install winetricks

```bash
sudo apt update
sudo apt install winetricks
```

## Install DirectX

I think version 9 is the minimum required, seems to work fine with 9 & 10 installed.

```bash
mark@pacifica:...Call of Duty 4 - Modern Warfare/bin> winetricks d3dx9
mark@pacifica:...Call of Duty 4 - Modern Warfare/bin> winetricks d3dx10
```

## Testing & Initial Config

Installed to: "/home/mark/.wine/drive_c/Program Files (x86)/Activision/Call of Duty 4 - Modern Warfare/"

Issue: It put a single-player and a multi-payer icon on the desktop.  Launching single-player errors: Can't find DVD-Rom.

Sol'n:
You can grab a patched iw3sp.exe file from a game torrent or elswhere.  The one with a md5 sum of `77d460bfbfff90bcf930ecc654588000` is known to work.  Use the appropriate command below to calculate an md5 sum.

```
# Linux\MacOS
md5sum [gamepath]/iw3sp.exe

# Windows (PowerShell or Command Prompt)
certutil -hashfile [gamepath]/iw3sp.exe MD5
```

1. Renamed "/home/mark/.wine/drive_c/Program Files (x86)/Activision/Call of Duty 4 - Modern Warfare/iw3sp.exe" to iws3sp.original.exe
2. Copied over iw3sp.exe from the torrented file.  Game now runs without disc.

Issue: Everything was really tiny (4K tv @ 10ft distance).

Sol'n:
Run winecfg, click emulate a virtual desktop, set resolution to 1920x1080p. Close winecfg.
In game, select Options-->Graphics.  Set Video Mode to 1080p or 4k (by clicking through).  Set DPI to ~200 (ok for a 65" 4K TV viewed at 10ft).

Issue: Desktop icons empty icons

Sol'n:
Apply proper icon to desktop shortcuts, and rename to "CoD4 Singleplayer" & "CoD4 Multiplayer"

## After installation, unmount ISO
```
sudo umount /mnt/iso
```
