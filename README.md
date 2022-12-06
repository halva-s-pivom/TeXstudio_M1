# TeXstudio_M1
TeXstudio compiled (with poppler) for Apple M1

If you are not scared of being hacked, here is the dmg:
https://drive.google.com/file/d/1xfFxPTWIT9c0aQ7EnP1WY5T50Awi25lt/view?usp=sharing
# Howto (briefly)
  1. Download poppler tarball from https://poppler.freedesktop.org/, extract it, build it and install system-wide.
  2. Install qt6 via brew.
  3. Clone TeXstudio and build it (`sh BUILD.sh`). If some packages are missing, install them via brew or however you wish and retry `sh BUILD.sh`.
# Howto (in detail)
1. Install qt6
    1. Open Terminal
    2. Type `brew install qt`
2. Install poppler
    1. Go to official poppler website https://poppler.freedesktop.org/ and download tarball (poppler-22.12.0.tar.xz) simply by clicking the link. 
    Assume you've downloaded it to ~/Downloads/; do the following:
    1. Open Terminal
    2. Type `cd ~/Downloads` and hit return
    3. Type `tar -xf poppler-22.12.0.tar.xz` and hit return
    4. Type `cd poppler-22.12.0` and hit return
    5. Type `sudo sh INSTALL` and hit return
3. Clone texstudio and build it:
    1. Open Terminal
    2. Type `cd ~/Downloads` and hit return
    3. Type `git clone https://github.com/texstudio-org/texstudio.git` and hit return
    4. Type `cd ~/Downloads/texstudio` and hit return
    5. Type `sh BUILD.sh` and hit return
    6. Choose build configuration provided (yes to poppler)
# My configuration
 1. TeXstudio 4.4.2
 2. compiled with Qt 6.4.0 R
 3. poppler-22.12.0
 4. MACOS 13.0.1
