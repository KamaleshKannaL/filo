# Third-party software

Filo is free to use (see `LICENSE`). It is built with the following software
under their own licenses.

## Built into Filo

| Component | License | Copyright |
|---|---|---|
| [Go](https://go.dev) standard library and runtime | BSD 3-Clause | The Go Authors |
| [golang.org/x/sys](https://pkg.go.dev/golang.org/x/sys) | BSD 3-Clause | The Go Authors |
| [fsnotify](https://github.com/fsnotify/fsnotify) | BSD 3-Clause | The Go Authors, fsnotify Authors |
| [fyne.io/systray](https://github.com/fyne-io/systray) | Apache License 2.0 | Fyne.io developers and contributors |
| [godbus/dbus](https://github.com/godbus/dbus) (Linux) | BSD 2-Clause | Georg Reinke, Google |
| [go-webview2](https://github.com/jchv/go-webview2) (Windows) | MIT | John Chadwick |
| [go-winloader](https://github.com/jchv/go-winloader) (Windows) | ISC | John Chadwick |

The full license texts ship with each component's source at the links above.

## Provided by your computer, not shipped with Filo

- **WebKitGTK** (Linux), LGPL 2.1, draws Filo's window.
- **Microsoft Edge WebView2 Runtime** (Windows), part of Windows 10 and 11, draws Filo's window.
