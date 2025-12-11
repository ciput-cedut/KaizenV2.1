# KaizenV2.1 - Monitor Input Switcher

A graphical user interface application for managing and switching monitor input sources on Windows. Built with Python and CustomTkinter.

## Features

- 🖥️ **Multi-Monitor Support** - Detect and manage multiple monitors simultaneously
- 🔄 **Input Source Switching** - Switch between different input sources (HDMI, DisplayPort, USB-C, Thunderbolt, etc.)
- 📊 **Monitor Information** - Display monitor brand, model, and current input source
- 🔍 **Auto-Detection** - Automatically detect available monitors and their supported inputs
- 🎨 **Modern UI** - Clean and intuitive interface built with CustomTkinter
- 📝 **Logging** - Detailed logging for troubleshooting

## Requirements

- Windows OS
- Python 3.8 or higher
- Administrator privileges (may be required for monitor control)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/ciput-cedut/KaizenV2.1.git
cd KaizenV2.1
```

2. Create and activate a virtual environment:
```powershell
py -m venv venv
.\venv\Scripts\Activate.ps1
```

3. Install dependencies:
```powershell
pip install -r requirements.txt
```

## Usage

Run the application:
```powershell
python monitor_manager.py
```

### How to Use:
1. Select a monitor from the dropdown menu
2. Select the desired input source
3. Click "Switch Input" to change the input
4. Use "Refresh" to reload monitor information

## Building Executable

To create a standalone executable file:

```powershell
pyinstaller --onefile --windowed --icon=monitor_manager_icon.ico monitor_manager.py
```

The executable will be created in the `dist` folder.

## Dependencies

- **customtkinter** - Modern UI framework
- **monitorcontrol** - Monitor DDC/CI control
- **screeninfo** - Screen information detection
- **screen-brightness-control** - Brightness and monitor control
- **pywin32** - Windows API access
- **pyedid** - EDID parsing
- **pyinstaller** - Create standalone executables

## Supported Input Sources

- DisplayPort (DP1, DP2)
- HDMI (HDMI1, HDMI2)
- USB-C
- Thunderbolt
- DVI
- Analog/VGA
- Component
- And more...

## Logging

The application creates a `monitor_manager.log` file in the project directory with detailed information about operations and any errors.

## Troubleshooting

- **Monitor not detected**: Ensure the monitor supports DDC/CI protocol
- **Cannot switch input**: Try running the application as administrator
- **Permission errors**: Some monitors may require elevated privileges

## Credits

**Created by:** LuqmanHakimAmiruddin@PDC

## License

This project is open source and available for personal and commercial use.

## Contributing

Contributions, issues, and feature requests are welcome!
