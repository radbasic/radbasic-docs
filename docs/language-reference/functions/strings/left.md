# Left

Returns a specified number of characters from the left side of a string.

---

## Left

Extracts characters from the beginning of a string.

**Syntax**

```basic
Left(string, length)
```

**Parameters**

| Parameter | Type | Description |
|---|---|---|
| string | String | The source string. |
| length | Integer | The number of characters to return. If greater than the length of `string`, the entire string is returned. |

**Return Value**

`String` — the leftmost `length` characters of `string`.

**Example**

```basic
Dim result As String
result = Left("Hello World", 5)
Print result   ' Output: Hello
```

---
