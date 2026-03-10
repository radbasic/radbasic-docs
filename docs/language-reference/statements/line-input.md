## Line Input #

Reads one line of text from an open sequential file and assigns it to a string variable. The line is read up to, but not including, the newline character.

#### Syntax

```basic
Line Input #fileNumber, varName
```

#### Parameters

- **fileNumber**: The file number used when the file was opened with `Open`.
- **varName**: A `String` variable that receives the line of text.

#### Remarks

- The file must be opened in `Input` mode.
- Each call reads the next line from the file.
- Unlike `Input #`, `Line Input #` reads the entire line as-is, preserving commas and quotation marks.
- Use `EOF(fileNumber)` to detect the end of the file before calling `Line Input #` to avoid a runtime error.

#### Example

```basic
Dim fileNum As Integer
Dim lineText As String

fileNum = FreeFile
Open "notes.txt" For Input As #fileNum

Do While Not EOF(fileNum)
    Line Input #fileNum, lineText
    Print lineText
Loop

Close #fileNum
```
