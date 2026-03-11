# Rnd

Returns a random `Single` value greater than or equal to 0 and less than 1.

---

## Rnd

Returns the next value from the random number sequence.

**Syntax**

```basic
Rnd[(number)]
```

**Parameters**

| Parameter | Type | Description |
|---|---|---|
| number | Single | Optional. Controls which random number is returned. If negative, returns the same number each time using `number` as the seed. If zero, returns the most recently generated number. If positive or omitted, returns the next number in the sequence. |

**Return Value**

`Single` — a value in the range [0, 1).

**Example**

```basic
Randomize
Dim i As Integer
For i = 1 To 5
    Print Int(Rnd * 100)   ' Output: 5 random integers between 0 and 99
Next i
```

---
