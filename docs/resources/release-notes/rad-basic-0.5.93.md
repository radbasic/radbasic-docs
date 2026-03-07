## RAD Basic 0.5.93 Pre-Beta 4 - Release Notes

RAD Basic Pre-Beta 4 release (0.5.93.0)

Pre-release of Beta 4
Notes: This is an early access to Beta version. 

### New

- [IDE] Added Show Logs and Collect Logs operations under Help Menu for troubleshooting problems.
- [IDE] Added formatting check in numeric values of Option Dialog and Project Properties Dialog.
- [IDE] Added configuration of editor's font and font-size.
- [IDE] Support to add/edit/save/remove BAS modules.
- [IDE] Support to add/edit/save/remove Class modules.
- [Compiler] Add support to #If...Then...#Else Directive (conditional compilation).
- [Compiler] Add support to #Const Directive (define conditional compiler constants).
- [Compiler] Defined RADBASIC, Win32 and Win64 const directives.
- [Compiler] Add initial support for IO (Open, Close, Line Input statements).
- [Compiler] Initial support of Class modules compilation.

### Improvements

- [IDE] Remember last folder visited for saving new items.
- [IDE] Added more internal log to help troubleshooting issues.
- [Compiler] Improve managing of unexpected errors in runtime/usercode.

### Fixes

- [IDE] Fix Clickable error in output window for syntax errors.
- [IDE] Fix bug in String syntax highlighting.
- [Compiler] Fix compiling process of projects with items (Forms, Modules, ...) in different directories.
- [Compiler] Fix compilation of procedures without explicit visibility (public/private).

### Known issues

- [IDE] Form Designer Grid: not drawn properly while user resizes form and some performance issues in certain edge cases.
- [IDE] FRX values (Icon, Pictures, ComboBox List, ...) are readonly values in Form Designer, as there issues saving into FRX file.
- [Compiler] UDT only support basic types as members.
- [Compiler] Variant type is not supported.
- [Compiler] Option Explicit is mandatory. Source code without option explicit will be supported in followings releases.