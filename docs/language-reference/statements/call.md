## Call Statement

#### Syntax

```vb
Call procedureName([argument1, argument2, ...])
```


#### Description

The Call statement is used to invoke Sub, Function, or Property procedures in Visual Basic. Although optional, it can improve code readability, especially when passing ByRef arguments or when you want to clearly indicate that a procedure call is being made.

    Note: In VB6, using Call requires that arguments be enclosed in parentheses. If you don't use Call, parentheses are only required if a return value is expected.

#### Parameters


- **procedureName**: The name of the procedure to be executed.

- **argument1, argument2, ...**: Optional list of expressions passed as arguments to the procedure. They must match in type and number with those defined by the procedure.

#### Examples


No return value (Sub):

```vb
Sub ShowMessage()
    MsgBox "Hello from a procedure."
End Sub

' Call using Call
Call ShowMessage

' Call without Call (also valid)
ShowMessage
```

With arguments:

```vb
Sub Greet(name As String)
    MsgBox "Hello, " & name
End Sub

Call Greet("Carlos")    ' Using Call with parentheses
Greet "Carlos"          ' Without Call, no parentheses
```

With return value (Function):

```vb
Function Add(a As Integer, b As Integer) As Integer
    Add = a + b
End Function

Dim result As Integer

result = Add(5, 10)      ' Without Call, return value is used

Call Add(5, 10)          ' Valid, but return value is discarded
```

#### Remarks


- The use of Call is optional and often redundant.

- If you use Call, you must enclose the arguments in parentheses, even if there are no arguments.

- It is not recommended to use Call when calling functions that return values, as the return value will be ignored.

#### See Also

[Sub Statement](rbdoc:language_reference:statements:sub)

Function Statement

MsgBox Function