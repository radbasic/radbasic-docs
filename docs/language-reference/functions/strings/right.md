# Right

Returns a specified number of characters from the right side of a string.

---

## Right

Extracts characters from the end of a string.

**Syntax**

```basic
Right(string, length)
```

**Parameters**

| Parameter | Type | Description |
|---|---|---|
| string | String | The source string. |
| length | Integer | The number of characters to return. If greater than the length of `string`, the entire string is returned. |

**Return Value**

`String` — the rightmost `length` characters of `string`.

**Example**

```basic
Dim result As String
result = Right("Hello World", 5)
Print result   ' Output: World
```

---
