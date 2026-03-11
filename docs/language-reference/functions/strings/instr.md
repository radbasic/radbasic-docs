# InStr

Returns the position of the first occurrence of one string within another.

---

## InStr

Searches for a substring inside a string and returns the 1-based position of the first match, or 0 if not found.

**Syntax**

```basic
InStr([start, ] string1, string2)
```

**Parameters**

| Parameter | Type | Description |
|---|---|---|
| start | Integer | Optional. The character position at which to begin the search. Defaults to 1. |
| string1 | String | The string to search in. |
| string2 | String | The substring to search for. |

**Return Value**

`Integer` — the 1-based position of the first match, or 0 if `string2` is not found.

**Example**

```basic
Dim pos As Integer
pos = InStr("Hello World", "World")
Print pos   ' Output: 7

pos = InStr(8, "Hello World", "o")
Print pos   ' Output: 0
```

---
