## RAD Basic 0.6.0 Pre-Beta 6 - Release Notes


RAD Basic Pre-Beta 6 release (0.6.0)

Pre-release of Beta 6
Notes: This is an early access to Beta version.

### New


- [Platform] New AutoUpdate module, easing stay updated. It is an experimental feature.
- [IDE] New Samples Explorer.
- [IDE] New Factorial sample featuring recursion.
- [Compiler] Add recursion support in functions.
- [Compiler] Check Option Explicit is on when compiles. Raise error if Option Explicit is Off, as it is not supported by compiler.


### Improvements

  *[IDE] Add missing icons in Form Layout.

### Fixes

  *[Compiler] Fix error in declaration of Sub/Function without explicit visibility (Private/Public keyword).

### Known issues


  *Installer and executables are not digitally signed because we are managing renovation of code signing certificate.
  *[IDE] Form Designer Grid: not drawn properly while user resizes form and some performance issues in certain edge cases.
  *[IDE] FRX values (Icon, Pictures, ComboBox List, ...) are readonly values in Form Designer, as there issues saving into FRX file.
  *[Compiler] UDT only support basic types as members.
  *[Compiler] Variant type is not supported.
  *[Compiler] Option Explicit is mandatory. Source code without option explicit will be supported in later releases.
