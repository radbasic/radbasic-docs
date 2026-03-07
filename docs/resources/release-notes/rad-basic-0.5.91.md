## RAD Basic 0.5.91 Pre-Beta 2 - Release Notes

RAD Basic Pre-Beta 2 release (0.5.91.0)

Pre-release of Beta 2

Notes: This is an early access to Beta 2 version.
 
### New
 
- New online installer digitally signed. Try to play more friendly with antivirus software.
- New OpenAI Chat sample.
- Change location of samples to user profile, avoiding issues with UAC.
- [Compiler] Add partial implementation of VB.App class.
- [Compiler] Implemented declaration and use of constants.
- [Compiler] Add VBA.Constants (vbNewLine, vbCrLf, ...).
- [Compiler] Implemented "Not" boolean operator.
- [Compiler] Implemented more functions of VBA.Strings: InStr, Len, Replace, LCase, UCase, Chr and Asc.
- [Compiler] Initial support of COM api (ActiveX). Implemented CreateObject function which creates and returns a reference to an ActiveX object in runtime (late binding).
- [IDE] Add comment/uncomment block operations.
- [IDE] Add Quick Search/Search and Replace operations.

### Improvements

- Shipped RAD Basic binaries are now digitally signed.

### Fixes

- [Compiler] On output compiler errors: fixed source code line calculation when there is not Option Module (as 'Option Explicit') and when there are syntax errors.
- [Compiler] Fix ExpressionSolver with edge cases in calling methods.
- [Compiler] Fix escape quote char in Strings.
- [Compiler] Add Click event in forms.
- [IDE] Fixed clickable compiler errors in output window when path contains parentheses.