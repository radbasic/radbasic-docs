## Print #

Writes formatted text to an open sequential file. The output format mirrors what the `Print` statement produces on screen.

#### Syntax

```basic
Print #fileNumber [, outputList]
```

#### Parameters

- **fileNumber**: The file number used when the file was opened with `Open`.
- **outputList**: One or more values to write, optionally separated by `,` or `;`.

#### Output separators

| Separator | Effect |
|---|---|
| `,` (comma) | Advances to the next print zone (column multiple of 14) |
| `;` (semicolon) | Writes the next value immediately adjacent, with no spacing |
| *(none)* | Writes the value followed by a newline |

#### Remarks

- The file must be opened in `Output` or `Append` mode.
- Strings are written without surrounding quotes. Use `Write #` instead if you need quoted, comma-delimited output suitable for re-reading with `Input #`.
- A trailing `;` suppresses the newline at the end of the line.

#### Example

```basic
Dim fileNum As Integer
fileNum = FreeFile
Open "report.txt" For Output As #fileNum

Print #fileNum, "Name", "Score"   ' Tab-separated columns
Print #fileNum, "Alice", 95
Print #fileNum, "Bob", 87

Close #fileNum
```
