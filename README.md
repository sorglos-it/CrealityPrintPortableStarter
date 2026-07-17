<<<<<<< HEAD
# CrealityPrintPortableStarter

<img src="CrealityPrint_192px.png" alt="Creality Print icon" width="96" align="right"/>

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Windows-blue.svg)](#requirements)
[![Donate](https://img.shields.io/badge/Donate-PayPal-00457C.svg?logo=paypal)](https://www.paypal.com/donate/?hosted_button_id=6CDEVZGJWTNQQ)

A tiny launcher that runs **[Creality Print](https://github.com/CrealityOfficial/CrealityPrint)** in **portable mode**.

Instead of storing your configuration in the Windows user profile (`%APPDATA%`), all profile settings are saved in a `profile` folder right next to the application — perfect for USB sticks, shared machines, or keeping multiple independent Creality Print setups side by side.

## Features

- ✅ Truly portable: all settings live in a local `profile` folder
- ✅ No installation, no registry entries, no admin rights required
- ✅ Take your printer profiles, filament presets, and settings with you on a USB drive
- ✅ Run multiple independent Creality Print configurations on the same PC

## Requirements

- Windows with [.NET Framework 4.7.2](https://dotnet.microsoft.com/download/dotnet-framework/net472) or newer (preinstalled on Windows 10/11)
- [Creality Print](https://github.com/CrealityOfficial/CrealityPrint/releases)
=======
# CrealityPrintPortable

[![Shell](https://img.shields.io/badge/shell-bash-89e051.svg)](#)
[![Platform](https://img.shields.io/badge/platform-Proxmox%20VE-e57000.svg)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Donate](https://img.shields.io/badge/Donate-PayPal-00457C.svg?logo=paypal)](https://www.paypal.com/donate/?hosted_button_id=6CDEVZGJWTNQQ)

Executable for running CrealityPrint in portable mode
Profile settings will be saved in `profile` folder
>>>>>>> 96dbb2e3e93f623c3d0a0ff16cbe59ce7787cdab

## Installation

1. Download and unzip **Creality Print** from the official releases page:
   [https://github.com/CrealityOfficial/CrealityPrint/releases](https://github.com/CrealityOfficial/CrealityPrint/releases)
2. Copy `CrealityPrintPortableStarter.exe` into your Creality Print folder
   (next to the original `CrealityPrint.exe`)
3. Run `CrealityPrintPortableStarter.exe`

That's it — Creality Print starts in portable mode, and a `profile` folder is created next to the executable to hold all of your settings.

## How it works

The starter simply launches Creality Print with the `--datadir` command line argument:

```
CrealityPrint.exe --datadir profile
```

This tells Creality Print to read and write all configuration data to the local `profile` folder instead of the current user's `%APPDATA%` directory.

## Building from source

1. Open `CrealityPrintPortable.sln` in Visual Studio (2017 or newer)
2. Select the **Release** configuration and build the solution
3. The executable is created in `CrealityPrintPortable\bin\Release\`

## Support this project ❤️

If this little tool saves you time, consider buying me a coffee:

[![Donate with PayPal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/donate/?hosted_button_id=6CDEVZGJWTNQQ)

**[➡️ Donate via PayPal](https://www.paypal.com/donate/?hosted_button_id=6CDEVZGJWTNQQ)**

## Credits

Based on [entrhopi/PrusaSlicerPortable](https://github.com/entrhopi/PrusaSlicerPortable), adapted for Creality Print.

Creality Print is developed by [Creality](https://github.com/CrealityOfficial/CrealityPrint). This project is not affiliated with or endorsed by Creality.

## License

This project is licensed under the [MIT License](LICENSE) — © 2025 Thomas Weirich.
