## RAD Basic 0.10.0 Pre-Beta 10 - Release Notes

RAD Basic Pre-Beta 10 release (0.10.0)

Notes: This is an early access to Beta version.

### New

- [IDE] Error highlighting applied to line-column, underlining only the relevant part of the statement.
- [Runtime] Implemented Property 'ShowInTaskbar' for Forms.
- [IDE] In New Project dialog: double click in project type icon executes the action.
- [IDE] Add New project shortcut in Start Page. Add icons in Open and New shortcuts.

### Improvements

- [IDE] If user cancels the save as dialog, form is not closed (avoid losing changes).

### Fixes

- [IDE] Changes in Form Properties modify the unsaved state.
- [IDE & Compiler] Fixes for load/save/compile projects with files with special chars (accents, ...).
- [Compiler] Fixed issues when FileName is different from Object Name.

### Known issues

- Due to internal rewrite of expressions evaluator, some bugs could be remaining.
- Installer and executables are not digitally signed because we are managing renovation of code signing certificate.
- [IDE] Form Designer Grid: not drawn properly while user resizes form and some performance issues in certain edge cases.
- [IDE] FRX values (Icon, Pictures, ComboBox List, ...) are readonly values in Form Designer, as there issues saving into FRX file.
- [Compiler] UDT only support basic types as members.
- [Compiler] Variant type is not supported.
- [Compiler] Option Explicit is mandatory. Source code without option explicit will be supported in followings releases.

