## RAD Basic 0.5.92 Pre-Beta 3 - Release Notes


RAD Basic Pre-Beta 3 release (0.5.92.0)

Pre-release of Beta 3
Notes: This is an early access to Beta version.
 
### New

- [IDE] Remember window state, size and location from last run and restore them when IDE starts.
- [IDE] Can edit project version info.
- [IDE] Add "Expand all nodes in Project Explorer on project load" feature.
- [IDE] Form Designer Grid and Align to Grid feature.
  *[IDE] Show control type in Control Properties list.
  *[Compiler] Add implementation of remaining intrinsic components: ListBox, ComboBox, Image and PictureBox.
  *[Compiler] Add support to manage FRX data added with Form Designer (ComboBox List Items).
  *[Compiler] Add support for Enumeration types (via Enum statement).
  *[Compiler] Add support for UDT (User Defined Types with Type statement).
  *[Compiler] Implemented FOR...NEXT statement.
  *[Compiler] Add support for END statement.
  *[Compiler] Add support for explicit procedure calls with Call keyword.
  *[Compiler] Implemented user Functions with Function keyword.
  *[Compiler] Implemented Do...Loop statement.
  *[Compiler] Implemented "Exit For", "Exit Do", "Exit Sub", "Exit Function" statements.
  *[Compiler] Optional and default value in Sub/Function parameters.
  *[Compiler] Add support of label marks in code (for OnError and Goto statements).
  *[Compiler] Initial implementation of error managing system (On Error Goto, Resume Next, etc.).
  *[Compiler] Fixed type of Value property of VB.CheckBox to CheckBoxConstants Enumeration.
  *[Compiler] Add AlignmentConstants and Alignment property to VB.Label.
  *[Compiler] Add PasswordChar and Locked properties to TextBox.
  *[Compiler] Add support for Window Icon in forms.
  *[Compiler] Write Exe icon and version info into compiled executable.
  *[Samples] Update OpenAI sample from davinci-3 model to ChatGPT3.

### Improvements

  *[IDE] Add modified flag and unsaved warning when a component is deleted in Form Designer.
  *[IDE] Show icons in Form Layout and select control with double-click.
  *[Compiler] Add modified flag and unsaved warning when a component is deleted in Form Designer.
  *[Compiler] Improve command line parser.

### Fixes

  *[IDE] Added missing keywords to highlighting of the code editor.
  *[IDE] Improve highlighting color for URL.
  *[IDE] Fixed state of pending unsaved changes in new Code Editor.
  *[IDE] Fixed regression in registering Click event in form object.
  *[IDE] Adding controls to forms respects "Visual Style" setting of the project.
  *[IDE] Show changes in Form Designer when change control properties.
  *[IDE] & [Compiler] Fixed encoding issues loading forms with accents and other non english text.
  *[IDE] Disable UAC virtualization via manifest. When tries to write to UAC protected folder (as %PROGRAM FILES%) it fails with error instead of saving to a virtual directory.

### Known issues


  *[IDE] Form Designer Grid: not drawn properly while user resizes form and some performance issues in certain edge cases.
  *[IDE] FRX values (Icon, Pictures, ComboBox List, ...) are readonly values in Form Designer, as there issues saving into FRX file.
  *[Compiler] UDT only support basic types as members.
  *[Compiler] Variant type is not supported.
  *[Compiler] Option Explicit is mandatory. Source code without option explicit will be supported in later releases.