# Randomize

Seeds the random number generator used by `Rnd`. Call this once at the start of your program to ensure a different sequence on each run.

---

## Randomize

Seeds the random number generator.

**Syntax**

```basic
Randomize [seed]
```

**Parameters**

| Parameter | Type | Description |
|---|---|---|
| seed | Variant | Optional. A numeric value used to initialize the random number generator. If omitted, uses the system timer. |

**Return Value**

None. This is a statement, not a function.

**Example**

```basic
Randomize
Dim roll As Integer
roll = Int(Rnd * 6) + 1
Print roll   ' Output: a random number between 1 and 6
```

---
