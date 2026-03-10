# What is RAD Basic?

RAD Basic is a modern compiler for the BASIC programming language, fully compatible with Visual Basic 6. It lets you open, compile, and run your existing VB6 projects without converting or rewriting any code.

---

## A modern compiler for VB6 code

RAD Basic is built from the ground up as an independent reimplementation of Visual Basic 6 — similar in spirit to how Wine reimplements the Windows API, or LibreOffice reimplements Microsoft Office file formats. No Visual Basic source code was used in its development.

The result is a compiler that understands VB6 syntax, respects VB6 behavior, and produces native Windows executables — without requiring any Microsoft runtime.

---

## Native VB6 file support

RAD Basic works directly with the files that VB6 produces:

| File type | Extension | Description |
|---|---|---|
| Project file | `.vbp` | The main project descriptor |
| Form module | `.frm` | Form code and layout |
| Standard module | `.bas` | General-purpose code modules |
| Class module | `.cls` | Object-oriented class definitions |

You open your existing `.vbp` project file and compile it directly. There is no conversion step, no migration wizard, and no need to restructure your project.

---

## No migration required

If your project compiles in VB6, it should compile in RAD Basic. The goal is 100% source-level compatibility: the same syntax, the same built-in functions, the same behavior.

This means you can:

- Open a project that was last touched in 1999 and compile it today.
- Make changes and improvements without learning a new language.
- Keep your existing codebase as-is and benefit from a modern compiler toolchain.

*Note: RAD Basic is under active development. Some VB6 features may not yet be implemented. Check the [Compatibility Matrix](../resources/compatibility-matrix.md) to see the current support status.*

---

## Native executables

Applications compiled with RAD Basic produce standard Windows PE executables. End users do not need to install any runtime — not the VB6 runtime, and not the .NET runtime. The output file runs on its own.

*Note: The RAD Basic IDE and compiler themselves require .NET to run on the developer machine. This is a build-time dependency only and does not affect the programs you produce.*

---

## Legal status

RAD Basic is a clean-room reimplementation. The development team has not accessed Visual Basic source code. RAD Basic is written in C and C#, using independent tools such as ANTLR for parsing. It is a legal product, in the same way that other compatibility-layer projects like Wine and ReactOS are legal.
