# Startup

This repo is for run webview on windows.
1. add WebView.MapDir for local files.
2. change hook namespace from window to window.eel, call hook function in format of eel.xxx instead.

# Usage
1. clone this repo
2. run build.bat in MSVC cmd, and you will got webview.*
3. put webview.* to root of your repo, or other path on demand
4. add the link flag to your code
```go
/*
#cgo windows LDFLAGS: -L${SRCDIR} -lwebview
*/
import "C"
import "github.com/codeindex2937/webview"
```
