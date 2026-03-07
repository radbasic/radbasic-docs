## RAD Basic 0.5.0 Alpha 3 - Release Notes


Third public release.

Notes: This release is focused in IDE user experience (especially in form designer). There is almost no new features in the compiler.
This release cycle was long due to the work done to fix Clang's external error that prevents it from compiling on certain machines.
  
### New

  - Added support for creating new projects (at this moment only Standard EXE).
  - Added support for adding, moving and removing controls in Form Designer.
  - Added new Form Layout tab.
  - Support for adding and removing forms in the project.
  - Incremental compiler: By default RAD Basic compiler only compiles modified files.
  - Added Rebuild all project menu item, to force regenerate all files and not use incremental compiler.
  - Added Clean project menu item, to clean generated files and force regenerate all files and not use incremental compiler.
  - Added pop-up menu in Project Explorer with most used actions.

### Improvements

  - Improved dramatically Form Designer.
  - Allows to resize the form.
  - Allows to change component property values from the properties tab.
  - Added Dynamic syntax coloring in code editor (for the next release, it will be replaced by a new LSP-based component with code completion features).
  - Warns before closing Form Designer/Code Editor if there are unsaved modifications.

### Fixes


  - Fixed memory crash when running internal clang compiler in some machines.
  - A lot of small fixes, improving general UX in IDE.