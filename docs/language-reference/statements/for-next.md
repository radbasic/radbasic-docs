## For...Next

Repeats a block of statements a fixed number of times, using a counter variable that increments (or decrements) after each iteration.

#### Syntax

```basic
For counter = start To end [Step stepValue]
    [statements]
    [Exit For]
Next [counter]
```

#### Parameters

- **counter**: A numeric variable used as the loop control variable.
- **start**: The initial value of `counter`.
- **end**: The final value of `counter`.
- **stepValue**: The amount added to `counter` after each iteration. Defaults to `1`.
- **statements**: One or more statements to execute inside the loop.

#### Remarks

- If `stepValue` is positive, the loop runs while `counter <= end`.
- If `stepValue` is negative, the loop runs while `counter >= end`.
- `Exit For` exits the loop immediately from any point inside it.
- Including the counter name after `Next` is optional but improves readability.

#### Examples

```basic
Dim i As Integer
For i = 1 To 5
    Print i
Next i
' Output: 1 2 3 4 5
```

```basic
' Count down using a negative Step
Dim i As Integer
For i = 10 To 1 Step -2
    Print i
Next i
' Output: 10 8 6 4 2
```
