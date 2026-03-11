# Sqr

Returns the square root of a number.

---

## Sqr

Computes the square root of a non-negative numeric expression.

**Syntax**

```basic
Sqr(number)
```

**Parameters**

| Parameter | Type | Description |
|---|---|---|
| number | Double | A non-negative numeric expression. |

**Return Value**

`Double` — the square root of `number`.

**Example**

```basic
Dim result As Double
result = Sqr(144)
Print result   ' Output: 12
```

!!! warning
    Passing a negative value to `Sqr` causes a runtime error. Validate input before calling this function if the value may be negative.

---
