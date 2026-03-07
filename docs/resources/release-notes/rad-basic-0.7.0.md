## RAD Basic 0.7.0 Pre-Beta 7 - Release Notes


RAD Basic Pre-Beta 7 release (0.7.0)

Notes: This is an early access to Beta version.

### New


- [IDE] Initial support of User Controls (readonly), cannot be modified yet.
- [Compiler] Initial support of User Controls compilation.
- [IDE] New User Control Project sample.
- [Compiler] Implemented Select Case statement.
- [Compiler] Implemented Visible and Enabled properties for: VB.CommandButton, VB.CheckBox, VB.ComboBox, VB.OptionButton and VB.TextBox.


### Improvements

  *[IDE] Double click in Form generate/edit Load event, as in VB6.
  *[Platform] Improvements in license manager.
  *[IDE] Open Dialog remember last folder used.

### Fixes

  *Fixed partially if a project has a file name with an special character (like ä,ö,ü, ...) the project can't be loaded

### Known issues


  *Installer and executables are not digitally signed because we are managing renovation of code signing certificate.
  *[IDE] Form Designer Grid: not drawn properly while user resizes form and some performance issues in certain edge cases.
  *[IDE] FRX values (Icon, Pictures, ComboBox List, ...) are readonly values in Form Designer, as there issues saving into FRX file.
  *[IDE] User Controls are not editable yet.
  *[Compiler] UDT only support basic types as members.
  *[Compiler] Variant type is not supported.
  *[Compiler] Option Explicit is mandatory. Source code without option explicit will be supported in later releases.