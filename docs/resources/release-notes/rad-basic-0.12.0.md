## RAD Basic 0.12.0 Pre-Beta 12 - Release Notes

RAD Basic Pre-Beta 12 release (0.12.0.0)

Notes: This is an early access to Beta version.

### New

- [Installer] Unified installer for Beta and Nightly builds.
- [Installer] Installer and binaries are now digitally signed to improve trustworthiness to SmartScreen, Windows Defender and other security applications.
- [Installer] Installer checks minimum MS Windows version (10 or later).
- [IDE] Add ODBC sources configuration (32-bit and 64-bit) to tools menu.
- [IDE] New Components window, which allows users to manage and organize components of the project.
- [IDE] New window which shows the mapping of VB6 legacy components and their RAD Basic equivalents.
- [IDE] Support rendering ActiveX Controls in Form Designer.
- [IDE] Support opening ActiveX Control projects.
- [IDE] Show scrollbar in Form Designer if the content exceeds the visible area.
- [IDE] Samples: New PDF Viewer sample (based on Acrobat PDF OCX control).
- [IDE] Samples: User Control compiling to ActiveX (outputs an OCX file).
- [IDE] Samples: Rich Textbox control.
- [Compiler] Support using visual ActiveX controls in forms.
- [Compiler] Support generating ActiveX controls (OCX files).
- [Compiler] Added unsupported statements to the compiler, so they are reported as "CE900 - Feature not supported yet" error and not as syntax errors.
- [Runtime] Implemented RB Data Grid as replacement for the legacy Data Grid control.
- [Runtime] Implemented ScaleTop, ScaleLeft and WindowState properties in Form.
- [Runtime] Implemented VBRUN.FormWindowStateConstants enum.

### Improvements

- [Compiler] Improved handling of library dependencies when generating native code.

### Fixes

- [IDE] Clickable errors in output window follow the scrollbar movement.
- [IDE] Scroll and redim issues in Control Toolbox.
- [Compiler] Read Module Option Base declaration and apply it to all arrays in the module.
- [Compiler] Fix calculation of array bounds (LBound, UBound) in multi-dimensional arrays.
- [Compiler] Fix bug in showing forms in certain scenarios during compilation.

### Known issues

- [Compiler] Due to internal rewrite of expressions evaluator, some bugs could be remaining.
- [IDE] Some features are only available at compile level. They will be in IDE in following releases.
- [IDE] Form Designer Grid: not drawn properly while user resizes form and some performance issues in certain edge cases.
- [IDE] FRX values (Icon, Pictures, ComboBox List, ...) are readonly values in Form Designer, as there issues saving into FRX file.
- [Compiler] UDT only support basic types as members.
- [Compiler] Option Explicit is mandatory. Source code without option explicit will be supported in followings releases.
