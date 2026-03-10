## Open

Opens a file for reading or writing. All file access requires a file to be opened first with a unique file number obtained from `FreeFile`.

#### Syntax

```basic
Open pathName For mode [Access access] As [#]fileNumber [Len = recLength]
```

#### Parameters

- **pathName**: A string with the full or relative path to the file.
- **mode**: Specifies how the file is accessed. One of: `Input`, `Output`, `Append`, `Binary`, `Random`.
- **access**: Optional. Restricts the allowed operations: `Read`, `Write`, or `Read Write`.
- **fileNumber**: An integer from 1 to 511 that identifies the open file. Use `FreeFile` to get a free number.
- **recLength**: Optional. For `Random` mode, the fixed record length in bytes.

#### Modes

| Mode | Description |
|---|---|
| `Input` | Opens an existing file for sequential reading |
| `Output` | Opens (or creates) a file for sequential writing; existing content is erased |
| `Append` | Opens (or creates) a file for sequential writing; new content is added at the end |
| `Binary` | Opens a file for unstructured byte-level access |
| `Random` | Opens a file for fixed-length record access |

#### Remarks

- Always call `Close #fileNumber` when done to flush buffers and release the file handle.
- Opening a file with `Output` truncates its existing contents. Use `Append` to preserve them.

#### Example

```basic
Dim fileNum As Integer
fileNum = FreeFile

' Write to a file
Open "output.txt" For Output As #fileNum
Print #fileNum, "Hello, World!"
Close #fileNum

' Read from the same file
fileNum = FreeFile
Open "output.txt" For Input As #fileNum
Dim lineText As String
Line Input #fileNum, lineText
Print lineText   ' Output: Hello, World!
Close #fileNum
```
