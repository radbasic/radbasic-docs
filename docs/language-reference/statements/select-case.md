## Select Case

Evaluates a single expression and executes the first matching `Case` block. Prefer this over a long chain of `If...ElseIf` when comparing one value against many options.

#### Syntax

```basic
Select Case testExpression
    Case expressionList
        [statements]
    [Case expressionList
        [statements]]
    [Case Else
        [statements]]
End Select
```

#### Parameters

- **testExpression**: The value to compare against each `Case`.
- **expressionList**: One or more match expressions separated by commas. Can be a single value, a range (`1 To 10`), a comparison (`Is > 100`), or a comma-separated list (`1, 3, 5`).
- **statements**: One or more statements to execute when the case matches.

#### Remarks

- Only the first matching `Case` block executes; execution does not fall through to the next case.
- `Case Else` executes when no other case matches.
- A single `Case` can list multiple values or ranges separated by commas.

#### Examples

```basic
Dim day As Integer
day = 3

Select Case day
    Case 1
        Print "Monday"
    Case 2
        Print "Tuesday"
    Case 3
        Print "Wednesday"
    Case 4, 5
        Print "Thursday or Friday"
    Case 6, 7
        Print "Weekend"
    Case Else
        Print "Invalid day"
End Select
' Output: Wednesday
```

```basic
Dim score As Integer
score = 82

Select Case score
    Case Is >= 90
        Print "A"
    Case 70 To 89
        Print "B"
    Case 50 To 69
        Print "C"
    Case Else
        Print "F"
End Select
' Output: B
```
