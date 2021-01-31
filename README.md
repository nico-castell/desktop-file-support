<h1 align="center">
  <br>
    <img src="https://raw.githubusercontent.com/nico-castell/desktop-file-support/main/assets/extension_icon.png" width="275" height="275" alt="logo">
  <br><br>
  Desktop File Support
  <br>
</h1>

<p align="center">
  <img alt="Lines of code" src="https://img.shields.io/tokei/lines/github/nico-castell/desktop-file-support?color=yellow&label=Lines%20of%20code">
  <img alt="GitHub commits since latest release (by date)" src="https://img.shields.io/github/commits-since/nico-castell/desktop-file-support/latest?color=yellow&label=Commits%20since%20last%20release">
  <img alt="GitHub" src="https://img.shields.io/github/license/nico-castell/desktop-file-support?color=yellow&label=License">
</p>

<blockquote align="center">Live long, and prosper. - Spock</blockquote>

This extension allows VS Code to highlight the syntax of a .desktop file,
much like in gedit.

<!-- <p align="center"> -->
  <img width="586" height="440" src="https://raw.githubusercontent.com/nico-castell/desktop-file-support/main/assets/screenshot.png" alt="logo">
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
