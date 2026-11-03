## RAD Basic 0.13.0 Pre-Beta 13 - Release Notes

RAD Basic Pre-Beta 13 release (0.13.0.0)

Notes: This is an early access to Beta version.

### New

- [IDE & Compiler] List of 32-bit to 64-bit conversions of third-party controls.
- [IDE] Modifications in the project components are now properly tracked (updated in the project file and in the Form Designer toolbox).
- [IDE] Added a Menu Designer for creating and managing menus of the forms/windows in the IDE (right-click on a form and select "Add Menu Bar").
- [Compiler] Implemented ReDim statement.
- [Runtime] Implemented Command function.
- [Runtime] Implemented RB Chart as replacement for the legacy MS Chart control.

### Improvements

- [IDE & Compiler] Improved handling of 64-bit builds and object references: new project profile added.
- [IDE] Moved Components window into a section in Project Properties Panel.
- [IDE] Changes in Project Name, Description and other project properties are now properly saved.
- [IDE & Compiler] Separate output directories for 32-bit and 64-bit builds.
- [Compiler] Duplicate compilation errors are no longer reported.

### Fixes

- [IDE] Fixed missing object reference error in certain scenarios when saving a project to disk.
- [IDE] Fixed an issue preventing access to forms, modules, and classes after creating and saving a new project.
- [IDE] Fixed saving modules (*.bas) and user classes (*.cls) with wrong encoding.
- [IDE] Fixed default value for internal attribute VB_Exposed.
- [IDE] Fixed corruption in forms when saving Font information.
- [Runtime] Fixed Resize event of forms not firing when the form was shown the first time.
- [Runtime] Fixed CStr (VBA.Conversion) conversion with some types.
- [Compiler] Fixed compilation bug when using UDT (User Defined Types) as a procedure parameter.
- [Compiler] Fixed error in expressions with arrays and parentheses.
- [Compiler] Fixed error when declaring variables in local scope with a type hint instead of the "As Type" form.
