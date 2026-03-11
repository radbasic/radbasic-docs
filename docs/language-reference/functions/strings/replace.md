# Replace

Returns a string with all occurrences of a substring replaced by another substring.

---

## Replace

Searches a string for a substring and replaces every occurrence with a new value.

**Syntax**

```basic
Replace(expression, find, replaceWith[, start[, count]])
```

**Parameters**

| Parameter | Type | Description |
|---|---|---|
| expression | String | The source string to search. |
| find | String | The substring to search for. |
| replaceWith | String | The string to substitute in place of each match. |
| start | Integer | Optional. The 1-based position in `expression` to begin searching. Defaults to 1. |
| count | Integer | Optional. The maximum number of replacements to perform. Defaults to -1 (all occurrences). |

**Return Value**

`String` — a copy of `expression` with the replacements applied.

**Example**

```basic
Dim result As String
result = Replace("Hello World", "World", "RAD Basic")
Print result   ' Output: Hello RAD Basic
```

---
