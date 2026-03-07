## RAD Basic 0.4.0 Alpha 2 - Release Notes

Second public release which will begin monthly release cycle.

Notes:

- There are great changes in internals of the compiler due to support for "Sub Main" as startup object, new Expression Solver and String Type Support. There are some regressions and incompatibilities that will be fixed in future versions.
- Timer Sample is not shipped in this release due to incompatibilities with new Expression Solver.

### New

    - Added initial implementation of new Form Controls:
      - CheckBox
      - OptionButton (Also known as Radio Button).
         *Frame.
    - Support for container and child controls.
    - Support for "Sub Main" as startup object.
    - More detailed information of Components Version in About Window.
    - New Control Showcase sample.
    - Added initial support for String type and concatenation of strings.
    - New Expression Solver in the compiler for resolving complex expressions.
    - Added IDE logging.

### Improvements


  - Object Explorer only is enabled if there is a project loaded.
  - Reduce compile warnings of RAD Basic Runtime (C implementation) from 150+ to 60.

### Fixes

  - Fix unable to compile projects when RAD Basic is installed in program files folder and Windows UAC is active.
  - Fix can not open Object Explorer if RAD Basic is installed in program files folder.
  - Fix control selection in screens with different DPI.
  - A lot of small bugfixes in the compiler.