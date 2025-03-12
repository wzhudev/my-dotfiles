# Windows Setup

## GUI Applications

Install VS Code using `winget`:

```powershell
winget install -e --id Microsoft.VisualStudioCode
```

Additionally, install the following applications to enhance usability (not directly related to development):

- **Microsoft PowerToys**: Install via the Microsoft Store for various productivity utilities.
- **[Window Switcher](https://github.com/sigoden/window-switcher)**: Allows switching between windows of the same application.

## Configuration

### Windows Terminal

After installing all necessary applications, update the `command` for the Ubuntu profile to:

```powershell  
wsl.exe ~ -d Ubuntu -- tmux  
```  

This will open the terminal with `tmux` running by default.  

### WSL

Place the [.wslconfig](./.wslconfig) file in your home directory. For reference, see this [documentation](https://github.com/microsoft/WSL/issues/10753#issuecomment-1814839310).

### PowerToys

Remap **Caps Lock** to **Left Ctrl** using PowerToys.

### Window Switcher

Save the [window-switcher.ini](./window-switcher.ini) file in the same directory as `window-switcher.exe`.
