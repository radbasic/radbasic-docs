## Compiler constants


RAD Basic defines constants for exclusive use with the #If...Then...#Else directive. These constants are functionally equivalent to constants defined with the #const directive except that they are global in scope, so they apply everywhere in the project.

These are the defined compiler constants by RAD Basic:

| Constant | Value | Meaning |
| --- | --- | --- |
| **RADBASIC** | **True** | Application compiled with RAD Basic. |
| **Win32** | **True** | Environment is 32-bit compatible. |
| **Win64** | **True** | Environment is 64-bit compatible. |

Because Win32 returns True in both 32-bit and 64-bit development platforms, it is important that the order within the #If...Then...#Else directive returns the desired results in your code. For example, because Win32 returns True in 64-bit (Win32 is compatible in Win64 environments), checking for Win32 before Win64 results in the Win64 condition never running because Win32 returns True. The following order returns predictable results:

```basic
#If Win64 Then 
' Win64=true, Win32=true
#ElseIf Win32 Then 
' Win32=true
#Else 
' !!!! 
#End If

```