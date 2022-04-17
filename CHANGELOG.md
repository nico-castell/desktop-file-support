# Change log

All significant changes to **Desktop File Support** will be documented here

- [Released](#released)
	- [Version v0.0.19 - *2022-04-17*](#version-v0019---2022-04-17)
	- [Version 0.0.18 - *2021-07-29*](#version-0018---2021-07-29)
	- [Version 0.0.17 - *2021-07-19*](#version-0017---2021-07-19)
	- [Version 0.0.16 - *2021-07-19*](#version-0016---2021-07-19)
	- [Version 0.0.14 - 0.0.15 - *2021-07-17*](#version-0014---0015---2021-07-17)
	- [Version 0.0.13 - *2021-02-24*](#version-0013---2021-02-24)
	- [Version 0.0.10 - 0.0.12 - *2021-02-19*](#version-0010---0012---2021-02-19)
	- [Version 0.0.9 - *2021-02-01*](#version-009---2021-02-01)
	- [Version 0.0.8 - *2021-01-31*](#version-008---2021-01-31)
	- [Version 0.0.7 - *2021-01-31*](#version-007---2021-01-31)
	- [Version 0.0.6 - *2021-01-31*](#version-006---2021-01-31)
	- [Version 0.0.5 - *2021-01-31*](#version-005---2021-01-31)
- [Pre-Releases](#pre-releases)
	- [Version 0.0.4 - *2021-01-30*](#version-004---2021-01-30)
	- [Version 0.0.3 [YANKED] - *2021-01-30*](#version-003-yanked---2021-01-30)
	- [Version 0.0.2 - *2021-01-09*](#version-002---2021-01-09)
	- [Version 0.0.1 - *2021-01-09*](#version-001---2021-01-09)

## Released
### Version [v0.0.19](https://github.com/nico-castell/desktop-file-support/releases/tag/v0.0.19) - *2022-04-17*
Added various snippets as a simple way to suggest multiple keys. Credit to @EmilySeville7cfg.

### Version [0.0.18](https://github.com/nico-castell/desktop-file-support/releases/tag/0.0.18) - *2021-07-29*
Fixed a typo in the README. Credit to @QWxleA.

### Version [0.0.17](https://github.com/nico-castell/desktop-file-support/releases/tag/0.0.17) - *2021-07-19*
Nothing special here, just a pair of bug fixes.
#### Fixed
- Numbers outside of the proper context (such as in URLs) are no longer highlighted.
- The `=` equals operator is no longer highlighted outside of the proper context.

### Version [0.0.16](https://github.com/nico-castell/desktop-file-support/releases/tag/0.0.16) - *2021-07-19*
This release remaps some of the scoping of the syntax highlighting, while fixing some bad behaviour.
#### Added
- Files that end with the `.theme` extension are now opened as desktop entries.
- The `CursorTheme` key was added for *index.theme* files.
#### Changed
- `[Desktop Entry]` lines are now mapped to `markup.heading` so comments don't make them harder to
	see.
- Typos like writing `Names` instead of `Name` now cause the entire key not to be highlighted,
	making typos easier to spot.
- `;` semi-colons are now scoped as `strong` (it's up to the theme to highlight them).
- Changed the rules for ***%*** arguments in the value of the `Exec` key, they're now scoped to
	`variable.language`, and they only highligh values allowed by the
	[specification](https://specifications.freedesktop.org/desktop-entry-spec/latest/ar01s07.html)
- Changed the textmate scope of freedesktop recognized categories for the `Categories` key. They're
	now scoped to `markup.bold`.
#### Fixed
- Short arguments (`-l`, `-s`) to commands in the `Exec` key are now highlighted.
- When you specify the language of keys such as `Name` and `Comment` by using `[]`, you no longer
	need to type the `=` operator to have syntax highlighting.
- Removed patterns that weren't useful.
- The categories recognized by freedesktop are no longer highlighted outside the `Categories` key.

### Version [0.0.14 - 0.0.15](https://gihtub.com/nico-castell/desktop-file-support/releases/tag/0.0.15) - *2021-07-17*
#### Added
- Support for missing keys (credit to @Luxcium).
- Support for extending the format by using `X-` as per the
	[specification](https://specifications.freedesktop.org/desktop-entry-spec/desktop-entry-spec-latest.html#extending).

### Version [0.0.13](https://github.com/nico-castell/desktop-file-support/releases/tag/0.0.13) - *2021-02-24*
#### Added
- Link to .desktop file specifications in the README.
- Contribution guidelines
- GitHub workflow to automatically deploy

### Version [0.0.10 - 0.0.12](https://github.com/nico-castell/desktop-file-support/releases/tag/0.0.12) - *2021-02-19*
#### Added
1. Added support for theme index files in GNOME.
#### Changed
1. Sizing of the icon in the README.
2. Style of Spock's quote in the README.

### Version [0.0.9](https://github.com/nico-castell/desktop-file-support/releases/tag/0.0.9) - *2021-02-01*
#### Fixed
Unspecified file extensions will no longer open as *.desktop*. Unless, as it has always been, the first line is `[Desktop Entry]`.

### Version [0.0.8](https://github.com/nico-castell/desktop-file-support/releases/tag/0.0.8) - *2021-01-31*
#### Added
1. Introduction of folding regions through `#region` and `#endregion`, although this isn't officialy part of *.desktop* files. It should be useful to you.
1. Additionally, snippets for `#region` and `#endregion` were added.

### Version [0.0.7](https://github.com/nico-castell/desktop-file-support/releases/tag/0.0.7) - *2021-01-31*
#### Added
Updated the documentation.

### Version [0.0.6](https://github.com/nico-castell/desktop-file-support/releases/tag/0.0.6) - *2021-01-31*
#### Added
Now the README's example image shows more of what the extension does.

### Version 0.0.5 - *2021-01-31*
This is the first official release of this extension.
#### Added
The extension finally has an icon.

---
## Pre-Releases

### Version 0.0.4 - *2021-01-30*
#### Fixed
Images in the marketplace now display correctly.

### Version 0.0.3 [YANKED] - *2021-01-30*
#### Added
Images in the documentation.
#### Fixed
Plain text files are no longer interpreted as .desktop.

### Version 0.0.2 - *2021-01-09*
#### Changed
1. Regex to capture comments
2. Regex to capture strings

### Version 0.0.1 - *2021-01-09*
#### Added
1. Syntax Highlighting.
2. Snippets.
