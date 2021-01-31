# Desktop File Support
[![GitHub repo size](https://img.shields.io/github/repo-size/nico-castell/desktop-file-support?color=yellow&label=Repository%20Size)](https://github.com/nico-castell/desktop-file-support)
[![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/nico-castell/desktop-file-support/latest?color=yellow&label=Commits%20since%20last%20release)](https://github.com/nico-castell/desktop-file-support/commits)
[![GitHub](https://img.shields.io/github/license/nico-castell/desktop-file-support?color=yellow&label=License)](LICENSE)

This extension allows VS Code to highlight the syntax of a .desktop file,
much like in gedit.

<!-- <p align="center"> -->
  <img width="586" height="390" src="https://github.com/nico-castell/desktop-file-support/blob/main/assets/screenshot.png">
<!-- </p> -->

##  Features
1. Syntax Highlighting for .desktop files
1. Snippet for .desktop files: A standard way to tell gnome to open a new
   window.
    ~~~
    Exec=/usr/share/code/code newwin # expands to:
    Exec=/usr/share/code/code --no-sandbox --new-window %F
    ~~~

##  Known Issues
1. The scoping of the syntax highlighting could be improved.

> Live long, and prosper  
> Spock
