## Sub Statement

#### Syntax

```vb
[Private | Public | Friend | Static] Sub procedureName([arglist])
    [statements]
End Sub
```

#### Description


The **Sub** statement declares a **procedure** that performs a task but does **not return a value**. A **Sub** can take zero or more arguments and can be defined at the module, class, or form level.

A **Sub** procedure is called using either the Call statement or by using its name directly. It is commonly used for code that performs actions, such as manipulating controls, validating input, or responding to events.

#### Parameters

- **Private | Public | Friend | Static**: Optional keywords that define the scope or behavior of the procedure:
- Private: Accessible only within the same module.
- Public: Accessible from other modules or forms.
- Friend: Accessible within the same project (used in class modules).
- Static: Variables inside the procedure retain their values between calls.
- **procedureName**: The name of the procedure. Must follow standard naming rules.
- **arglist**: Optional. A comma-separated list of parameters passed to the procedure. Each argument may include:
  - ByVal (passed by value)
  - ByRef (passed by reference — default)
- A data type (e.g., As Integer, As String)
- statements: The block of code to execute when the procedure is called.
