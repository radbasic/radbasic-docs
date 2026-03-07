## RAD Basic 0.8.0 Pre-Beta 8 - Release Notes

RAD Basic Pre-Beta 8 release (0.8.0)

Notes: This is an early access to Beta version.

### New


- [IDE] Create and edit User Controls from IDE.
- [IDE] Allows change startup object in project properties.
- [IDE] New setting: Open startup object on project load.
- [Compiler] Initial support for hexadecimal values in properties.
- [Compiler] Introduction of warnings: Warn when a method signature is an event not defined (object or event not exists).
- [Compiler] Initial implementation of Output mode for files and Print statement.


### Improvements

  *[IDE] In Samples Explorer, double click open the selected sample.

### Fixes

  *[IDE] Fixed error "The configuration file has been changed by another program" which prevents to close the IDE when there are two instances opened.
  *[Compiler] Fixed compilation errors of Optional/Default values in Subs/Functions in certain situations.
  *[IDE] Fixed project temp path after saved a new created project.


### Known issues


  *Installer and executables are not digitally signed because we are managing renovation of code signing certificate.
  *[IDE] Form Designer Grid: not drawn properly while user resizes form and some performance issues in certain edge cases.
  *[IDE] FRX values (Icon, Pictures, ComboBox List, ...) are readonly values in Form Designer, as there issues saving into FRX file.
  *[IDE] User Controls are not editable yet.
  *[Compiler] UDT only support basic types as members.
  *[Compiler] Variant type is not supported.
  *[Compiler] Option Explicit is mandatory. Source code without option explicit will be supported in later releases.