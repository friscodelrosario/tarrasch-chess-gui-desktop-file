# tarrasch-chess-gui-desktop-file
Linux desktop entry file to generate executable icon after building from source 

## What is Tarrasch Chess GUI

[Tarrasch Chess GUI](https://github.com/billforsternz/tarrasch-chess-gui) is described by its developer as a "simple desktop chess workbench", enabling PGN production (with its own database), multiple UCI for analysis and play (why does anyone do that these days).

I've found Tarrasch GUI to be the best chess writing tool available for desktops (on Android, Chess PGN Master is shockingly good). Tarrasch GUI was a Windows project at first, eventually finding its way to Macintosh and Linux. 

## What's this desktop file?

If you build Tarrasch from source on Linux, you're left to launch it from command line, or futz with launcher items. Saving a .desktop file to /usr/share/applications generates an executable icon, and if you copy this one, maybe you'll save the time I spent digging for desktop environment [documentation](https://specifications.freedesktop.org/desktop-entry-spec/desktop-entry-spec-latest.html). 

Download/copy/clone tarrasch.desktop. Change the Exec to point at your Tarrasch in your base directory, and Icon to point at one of the application icons in your_base_dir/src/. Change Comment at will. Save it in /usr/share/applications. 

There's a utility for verifying desktop files: [desktop-file-validate](https://manpages.ubuntu.com/manpages/focal/en/man1/desktop-file-validate.1.html).

```
[Desktop Entry]
Version=1.0
Name=TarraschChessGUI
Comment=Surrender Dorothy
Exec=/home/frisco/tarrasch-chess-gui/tarrasch
Icon=/home/frisco/tarrasch-chess-gui/src/Tarrasch4Squares.ico
Terminal=false
Type=Application
Categories=Utility;Application;
```
## Will using Tarrasch Chess GUI help me get better at chess?

If you use it for playing through master games while guessing the winner's moves, or for endgame study, sure. Probably not if you use it for something dumb like compiling an opening database. 