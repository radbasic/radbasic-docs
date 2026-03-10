## While...Wend

Repeats a block of statements as long as a condition remains `True`. The condition is evaluated at the top of the loop before each iteration.

#### Syntax

```basic
While condition
    [statements]
Wend
```

#### Parameters

- **condition**: A Boolean expression evaluated before each iteration. The loop exits when it becomes `False`.
- **statements**: One or more statements to execute inside the loop.

#### Remarks

- If `condition` is `False` on the first evaluation, the body never executes.
- `While...Wend` does not support early exit. Use `Do...Loop` with `Exit Do` when you need to break out of the loop before the condition changes.

#### Example

```basic
Dim n As Integer
n = 1
While n <= 5
    Print n
    n = n + 1
Wend
' Output: 1 2 3 4 5
```
