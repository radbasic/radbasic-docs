## RAD Basic 0.11.0 Pre-Beta 11 - Release Notes

RAD Basic Pre-Beta 11 release (0.11.0.0)

Notes: This is an early access to Beta version.

### New

- [Installer] New Installer developed with RAD Basic itself.
- [IDE] Contents of Output Window are written to the log file, helping troubleshoot issues.
- [Compiler] Implemented DLL call with Declare Statement.
- [Compiler] Implemented remaining types: Byte, Date, Variant and Any (used in dll calls).
- [Compiler] Added support for applications with Menus defined in more than one form.
- [Compiler] Implemented String functions: LTRIM, RTRIM and TRIM.
- [Compiler] Implemented missing IO support (Append mode when writing files, FreeFile function).
- [Compiler] Implemented VBA.FileSystem functions and statements: Dir, MkDir, RmDir.
- [Compiler] Implemented VBA.DateTime functions and properties: Now.
- [Compiler] Implemented VBA.Interaction function: Environ.
- [Compiler] Implemented With statement.
- [Compiler] Implemented MID statement (left operation to substitute characters in string) in addition of already implemented MID function.
- [Compiler] Added support using MID with typehint (ending with $ character).
- [Compiler] Added support inferring the type from the typehint.
- [Compiler] Added support Me keyword for reference the object itself.
- [Compiler] Added support calling procedures with left parameters omitted (optional) in the call, but there are more parameters after them.
- [Runtime] Implemented Common Controls library: ProgressBar, Slider, TreeView.
- [Runtime] Implemented Common Dialog library: OpenDialog, SaveDialog.
- [Runtime] Implemented RichTextBox library.
- [Runtime] Implemented MDI (Multi Document Interface) support.
- [Runtime] Implemented Colors properties in intrinsic controls: Form, TextBox and Label.
- [Runtime] Implemented Border Style property in intrinsic controls: Form, Frame, Image,...
- [Runtime] Implemented Cancel and Default properties in Command Buttons.
- [Runtime] Implemented Font property in Label.
- [Runtime] Implemented support for more events: Activate, Load and Resize events in Forms.
- [Runtime] Implemented new method in Forms: Hide.
- [Runtime] Property 'Name' in controls is now accessible in runtime.
- [Runtime] Property 'Tag' in all controls.
- [Runtime] Implemented more Maths functions: Rnd() and Randomize().
- [Runtime] Implemented more Conversion functions (package VBA.Conversion): Int() and Fix().

### Improvements

- [IDE] Improve logging in IDE.
- [Compiler] Improvements in expression evaluator.
- [Compiler] Supports "+" operator for string concatenation.
- [Runtime] Improved conversion between different numeric types.

### Fixes

- [IDE & Compiler] Fixes for load/save/compile projects in directories with dots.
- [IDE] When compiling a project, the project and its items are no longer saved automatically; they are now saved only if changes have been detected.
- [IDE] F7 shortcut (show code) now works properly when the form is shown automatically when the project is opened.
- [Compiler] Fixed type conversion in string concatenation.
- [Compiler] Fixed using String and dates without explicit initialization.
- [Compiler] Fixed boolean conversion to string when using literals ("true" or "false").
- [Compiler] Fixed support of hexadecimal values in expressions and constants.
- [Compiler] Fixed error in expressions mixing functions (their return value) and variables/constants.
- [Compiler] Fixed error using NOT operator in inline IF statements (if without statements block).
- [Compiler] Fixed compilation error using user types with private visibility.
- [Compiler] Fixed compilation error in inline If statement (if in one line, without "end if" block).
- [Compiler] Fixed errors in enum usage introduced by new Expression Evaluator.
- [Compiler] Fixed issues nesting UDT inside other UDTs (User Defined Types with Type statement).
- [Runtime] In CommandButton controls, when text is larger than the control, it is now properly wrapped vertically (as VB6 does).
- [Runtime] Fixed click event do not fire when the control is a child of Frame control.

### Known issues

- Due to internal rewrite of expressions evaluator, some bugs could be remaining.
- Some features are only available at compile level. They will be in IDE in following releases.
- Installer and executables are not digitally signed because we are managing renovation of code signing certificate.
- [IDE] Form Designer Grid: not drawn properly while user resizes form and some performance issues in certain edge cases.
- [IDE] FRX values (Icon, Pictures, ComboBox List, ...) are readonly values in Form Designer, as there issues saving into FRX file.
- [Compiler] UDT only support basic types as members.
- [Compiler] Option Explicit is mandatory. Source code without option explicit will be supported in followings releases.
