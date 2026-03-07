## RAD Basic 0.5.90 Pre-Beta 1 - Release Notes

RAD Basic Pre-Beta 1 release (0.5.90.0)

Pre-release of Beta 1

Notes: This is an early access to Beta 1 version.
 
### New


- Compiler: Rewritten part of the core implementing multi-pass compiler. So, now we will be able to compile source code with methods calling other methods written after them.
- Compiler: Support for multiple variable declarations in single Dim statement.
- Compiler: Support for visibility modifier (Public, Private, ...) for procedures and variables.
- Compiler: Support for additional intrinsic data types: Single, Double and Boolean.
- Compiler: Support Boolean operators: 'And' and 'Or'.
- Compiler: Added basic string manipulation: concatenation with & symbol, and methods Left, Mid, Right and CInt.
- IDE: Add context menu to output window of RAD Basic IDE with "Copy" and "Clear All" actions.
- IDE: Add actions to context menu of Project Explorer: Open in File Explorer, Copy Full Path and Open in Terminal.
- IDE: New source code editor: with line numbers and code folding.
- IDE: Go to line menu item.
- IDE: Clickable errors in output window which allows to jump to line.

#### Improvements

- IDE: Improved dark theme.
- Added unit testing in IDE (as we had in compiler) and integration tests along e2e tests. These improvements helped to fix a lot of small bugs.

#### Fixes

- IDE: Fixed various bugs about saving form operation.
- IDE: Fixed not losing menu definition on the form when saving.
- IDE: Fixed show correctly containers/children in form layout window.
- IDE: Fixed bugs in loading/saving VBP, FRM and BAS modules files.
- IDE and compiler: Fixed a lot of small bugs.
- Compiler: Check members of an object are callable (not a property) when invoking it.
- Compiler: Ignoring case when resolving symbols.
- Compiler: Fix read properties.
- Compiler: Add a lot of missing checks and fixed small bugs.