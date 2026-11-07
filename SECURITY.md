# Security

## Reporting a problem

Please report security issues privately through GitHub:
**Security → Report a vulnerability** on this repository. Don't open a public
issue for them. You'll get an answer within a week.

## What Filo does on your computer

- **No network access.** Filo never connects to the internet: no analytics,
  no update checks, no accounts. The only network use is a server on
  `127.0.0.1` (your own computer) that shows Filo's window. Only Filo's own
  window can open it; other programs and other users on the computer can't.
- **Files it moves:** only loose files directly inside the folders you add,
  into subfolders of that same folder. It never deletes or overwrites a file,
  and never touches folders you drop in or files that are still downloading.
- **Files it writes:** its settings and a log of moves in your user config
  folder (`%AppData%\Filo` on Windows, `~/.config/Filo` on Linux), and a
  start-at-sign-in entry when you turn that on. On Linux it also adds itself
  to your apps menu (`~/.local/share/applications/filo.desktop`).
- **Programs it runs:** your file manager when you choose Show, and the
  system folder picker.

## Checking a download

Every release lists SHA-256 checksums in `SHA256SUMS`. To check a file:

```sh
sha256sum -c SHA256SUMS --ignore-missing                       # Linux
Get-FileHash Filo-v1.0.3-windows.exe -Algorithm SHA256         # Windows PowerShell
```

The result must match the line for that file in `SHA256SUMS`.
