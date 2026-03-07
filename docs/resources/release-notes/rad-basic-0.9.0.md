## RAD Basic 0.9.0 Pre-Beta 9 - Release Notes

RAD Basic Pre-Beta 9 release (0.9.0)

Notes: This is an early access to Beta version.

### New

  - [IDE] Compiler errors are shown in Editor with red underline decoration.
  - [IDE] Added "Restore samples" button in Options dialog. Now, you can undo your changes made in RAD Basic shipped samples, resetting them.
  - [IDE] Replaced the ChatGPT integration sample with a basic Excel automation example using COM dispatch calls, as the ChatGPT API is no longer free.
  - [Compiler & IDE] Added support for environment variable for path location and make it default.
  - [Compiler & IDE] Added support for recovering when a compiler error is found in source code (default mode). Now all errors in source code are listed. Can be switched back to VB6 style: Stop at any error in source.
  - [Compiler] New internal Expression System. It fixes a lot of bugs.
  - [Compiler] New Array implementation, more COM/ActiveX friendly:
    - Same internal layout as SafeArray (used in COM/OCX)
    - Fix use in expressions
    - Multidimensional support.
  - [Compiler] Added Let keyword support in assignments (explicit use of the Let keyword is a matter of style, but it is usually omitted).
  - [Compiler] Added support for read properties:
    - VB.CommandButton: Top, Left, Width, Height, Caption, Visible.
    - VB.Label: Top, Left, Width, Height, Caption, Visible.
    - VB.TextBox: Top, Left, Width, Height, Visible, Enabled.
    - VB.ComboBox: Top, Left, Width, Height, Visible, Enabled.
    - VB.Frame: Top, Left, Width, Height, Caption, Visible.
    - VB.Image: Top, Left, Width, Height.
    - VB.ListBox: Top, Left, Width, Height.
    - VB.OptionButton: Top, Left, Width, Height, Value, Caption, Visible, Enabled.
    - VB.PictureBox: Top, Left, Width, Height.
  - [Compiler] Fix use of parentheses in expressions.
  - [Compiler] Added Support of literal suffixes: "&" for Long literals, "!" for Single literals.
  - [Compiler] Implemented GoTo Statement.
  - [Compiler] Added new Math Operators:
    - Mod operator.
    - Pow operator (^).
    - Square root function (sqr).
  - [Compiler & Runtime] Moved conversion from Twips to Pixels into runtime (in compile-time using always twips).
  - [Runtime] VB.App.Path works as VB6 does: VBP file when running the application from the development environment or the path of the executable file when running the application as an executable file (outside IDE). 
  - [Runtime] Add functions for arrays: UBound and LBound.
  - [Runtime] MsgBox: Implemented all parameters and enums (helpFile and context are ignored at this moment).
  - [Runtime] Implemented functions from VBA.Conversion: CStr, CBool, CDbl, CInt, CLng and CSng.
  - [Runtime] Implemented "DoEvents" function.

### Improvements

- [IDE] Changes in control and form names are updated dynamically in form layout and project explorer.
- [Compiler] Rebuild/Clean now removes all files in build directory.
- [Compiler & Runtime] Better management of lifecycle of application Forms/Windows.

### Fixes

- [IDE] Fixed crash when saving non form items.
- [IDE] Fixed issues in some samples projects.
- [Compiler] Fixed a regression that caused the compilation of user-defined classes to fail.
- [Compiler] Fixed not interpreted "\" character in VB Strings as scape character.
- [Compiler] Projects with "Sub Main" as Startup Object finish right (won't get stuck in memory forever).
- [Compiler] Procedures containing "_" (event name construction), not failing to compile if some part don't exists (report a warning instead).
- [Compiler] Fixed comparison of strings in some expressions don't use the right function internal operator.
- [Compiler] Lots of small bugs fixed.

### Known issues

- Due to internal rewrite of expressions evaluator, some bugs could be remaining.
- Installer and executables are not digitally signed because we are managing renovation of code signing certificate.
- [IDE] Form Designer Grid: not drawn properly while user resizes form and some performance issues in certain edge cases.
- [IDE] FRX values (Icon, Pictures, ComboBox List, ...) are readonly values in Form Designer, as there issues saving into FRX file.
- [Compiler] UDT only support basic types as members.
- [Compiler] Variant type is not supported.
- [Compiler] Option Explicit is mandatory. Source code without option explicit will be supported in followings releases.

