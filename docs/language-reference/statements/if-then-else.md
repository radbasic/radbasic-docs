## If...Then...Else

Conditionally executes a block of statements based on the value of a Boolean expression.

#### Syntax

```basic
' Block form
If condition Then
    [statements]
[ElseIf condition2 Then
    [statements]]
[Else
    [statements]]
End If

' Single-line form
If condition Then statement [Else statement]
```

#### Parameters

- **condition**: A Boolean expression to evaluate.
- **statements**: One or more statements to execute when the condition is met.

#### Remarks

- Multiple `ElseIf` branches can appear between `If` and `Else`.
- Only the first branch whose condition is `True` executes.
- The `Else` branch executes when none of the preceding conditions are `True`.
- In the single-line form, `End If` is not used and only one statement may follow `Then` or `Else`.

#### Examples

```basic
Dim score As Integer
score = 75

If score >= 90 Then
    Print "A"
ElseIf score >= 70 Then
    Print "B"
ElseIf score >= 50 Then
    Print "C"
Else
    Print "F"
End If
' Output: B
```

```basic
' Single-line form
Dim x As Integer
x = 10
If x > 0 Then Print "Positive" Else Print "Non-positive"
```
