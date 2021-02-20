<h1 align="center">
  <br>
    <img src="https://raw.githubusercontent.com/nico-castell/desktop-file-support/main/assets/extension_icon.png" width="220" height="220" alt="logo">
  <br>
  Desktop File Support
</h1>

<p align="center">
  <img alt="Visual Studio Marketplace Version" src="https://img.shields.io/visual-studio-marketplace/v/nico-castell.linux-desktop-file?color=yellow&label=Version&style=flat-square">
  <img alt="GitHub commits since latest release (by date)" src="https://img.shields.io/github/commits-since/nico-castell/desktop-file-support/latest?color=yellow&label=Commits%20since%20last%20release&style=flat-square">
  <img alt="GitHub" src="https://img.shields.io/github/license/nico-castell/desktop-file-support?color=yellow&label=License&style=flat-square">
  <img alt="Lines of code" src="https://img.shields.io/tokei/lines/github/nico-castell/desktop-file-support?color=yellow&label=Lines%20of%20code&style=flat-square">
  <br><b>Live long, and prosper.<br>- Spock</b>
</p>

## Normal .desktop file
This extension allows VS Code to highlight the syntax of a .desktop file, much like in gedit.

<!-- <img width="625" height="440" src="assets/code-screenshot.png" alt="logo"> -->
<img width="625" height="440" src="https://raw.githubusercontent.com/nico-castell/desktop-file-support/main/assets/code-screenshot.png" alt="logo">

## Theme Index Files
Additionally, this extension highlights `[X-GNOME-Metetheme]` and it's keys

<!-- <img width="625" height="303" src="assets/theme-screenshot.png"> -->
<img width="625" height="303" src="https://raw.githubusercontent.com/nico-castell/desktop-file-support/main/assets/theme-screenshot.png">
<!-- This GNOME theme is found at: https://www.gnome-look.org/p/1253385/ -->

##  Features
1. Syntax Highlighting for .desktop files.
2. Extra syntax highlighting for [Theme Index files](https://people.gnome.org/~shaunm/admin-guide/themes-17.html).
3. Snippet for .desktop files: A standard way to tell gnome to open a new window.
    ```
    Exec=/usr/share/code/code newwin # expands to:
    Exec=/usr/share/code/code --no-sandbox --new-window %F
    ```
4. Folding regions through the use of `#region` and `#endregion`. This is not officially part of *.desktop* files, but it should help you.

##  Known Issues
1. The scoping of the syntax highlighting could be improved.
