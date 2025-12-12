
# ogg-winmm CD Audio Emulator for Worms 2 Frontend

## Info
- This project (originally by Hifi) uses .ogg music files on the disk to emulate CD tracks, replacing the need to have a CD in the drive to play music in certain games. GOG uses a modified version for several of their games. 
- bangstk's fork added improvements, such as Windows 10 support.
- maximilien-noal's fork made the project buildable with VS2017. They also added fixes for Wipeout 2097 and Virtua Fighter 2 which could also apply to other games.
- This fork is specific for Worms 2 with volume control and loading of FrontendKitWS modules. It also has updated libraries of libogg and libvorbis. It is included in [Worms 2 Plus](https://github.com/Carlmundo/W2-Plus).

## Build
- Open WinmmOgg with Visual Studio 2015 or newer.
- Run Build -> Build Solution (or Ctrl-Shift-B).

## Requirements
- Windows 8.1 SDK and headers installed for the build to succeed.
- *x86* 2017 MSVC Runtime for this wrapper to run.

## Usage
Copy "winmm.dll" into the same folder as the executable of the game you want to emulate CD music for.
In the same folder, make a "Music" subdirectory. Place the recorded music files from the disk as track02.ogg, track03.ogg, and so on in this Music folder. Remember, it starts with track02!

Now, instead of playing music from the CD, the game will play music from these files instead.