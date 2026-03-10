## Do...Loop

Repeats a block of statements while a condition is true, or until a condition becomes true. The condition can be evaluated at the beginning or end of the loop.

#### Syntax

```basic
' Condition at the top
Do [{While | Until} condition]
    [statements]
    [Exit Do]
Loop

' Condition at the bottom
Do
    [statements]
    [Exit Do]
Loop [{While | Until} condition]
```

#### Parameters

- **condition**: A Boolean expression evaluated before or after each iteration.
- **statements**: One or more statements to execute inside the loop.

#### Remarks

- `Do While` keeps looping as long as `condition` is `True`.
- `Do Until` keeps looping as long as `condition` is `False`.
- When the condition is placed after `Loop`, the body always executes at least once.
- `Exit Do` exits the loop immediately from any point inside it.

#### Examples

```basic
Dim n As Integer
n = 1
Do While n <= 5
    Print n
    n = n + 1
Loop
' Output: 1 2 3 4 5
```

```basic
Dim answer As String
Do
    answer = InputBox("Type YES to continue:")
Loop Until answer = "YES"
```
