# wry standalone

This is an attempt to bring WRY/Tauri to a standalone compiled binary allowing you to run a project and compile (embed the assets) into the binary without touching rust.

## Installation 

### Shell (Mac, Linux):
```bash
curl -fsSL https://raw.githubusercontent.com/lemarier/wry_standalone/main/scripts/install.sh | sh
```

### PowerShell (Windows):
```bash
iwr https://raw.githubusercontent.com/lemarier/wry_standalone/main/scripts/install.ps1 -useb | iex
```

### Clone sample repo
```bash
git clone https://github.com/lemarier/wry_demo.git
cd wry_demo
wry run ./main.js
wry compile ./main.js
ls -lah compiled-bin-test
```

### Create self contained binary
For test purpose it shuld generate a self contained binary as `compiled-bin-test` in the current directory.
```bash
wry compile ./main.js
```

#### Run the self contained binary
``` bash
./compiled-bin-test
```