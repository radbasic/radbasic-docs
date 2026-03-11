# Mid

Returns a substring from within a string.

---

## Mid

Extracts a portion of a string starting at a specified position.

**Syntax**

```basic
Mid(string, start[, length])
```

**Parameters**

| Parameter | Type | Description |
|---|---|---|
| string | String | The source string. |
| start | Integer | The 1-based position of the first character to return. |
| length | Integer | Optional. The number of characters to return. If omitted, returns all characters from `start` to the end of the string. |

**Return Value**

`String` — the extracted substring.

**Example**

```basic
Dim result As String
result = Mid("Hello World", 7, 5)
Print result   ' Output: World
```

---
