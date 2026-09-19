# NWN Include Documenter

VB6 NWScript documenter (project Project1, startup `Sub Main` in `Module1`) that parses Bioware `NWSCRIPT.NSS` under `c:\temp\NWN` and emits `NWNFunctions2.xml`. It harvests `//` and `/* */` comment blocks ahead of `void`/`int`/`action`/`effect`/… declarations, strips copyright boilerplate, and records function name, return type, parameters, prototype, and comments into an `<nwn_functions>` XML document (header notes export from NWSCRIPT.NSS v1.21, Jul 2002). Form1 is an empty shell; real work is in the module (repo ships `Module1.bas.example` with email redacted).

**Source last updated:** 2026-08-27 · **Language:** VB6 · **Target:** VB6 Win32 · **Output:** WinForms exe

_Note: original OneDrive LastWriteTime values were wiped to 2026-08-27 by a zip transfer; date above uses best available evidence (headers/copyright where helpful)._

## Solution structure

| Project | Language | Type | Purpose |
|---------|----------|------|---------|
| `Project1` (`Include Documenter.vbp`) | VB6 | WinForms exe | Parse NWSCRIPT.NSS comments/prototypes to XML |

## How to open

Open the `.vbp` in Visual Basic 6.0 IDE:
- `Include Documenter.vbp`

Restore `Module1.bas` from `Module1.bas.example` (rename) before building; credentials in the example are redacted.

## Requirements

- Visual Basic 6.0 IDE
- Bioware `NWSCRIPT.NSS` (and optional other `*.NSS`) under `c:\temp\NWN`

## Attribution and provenance

Working copy from Dave Robinson's OneDrive Historical Dev folder `VB/Old/NWN Include Documenter`.
Documents Bioware Neverwinter Nights NWScript API; XML header attributes Dave Robinson, 27 July 2002.

## License

MIT (c) 2026 VaderConsulting for Dave Robinson's code. See `LICENSE`.
