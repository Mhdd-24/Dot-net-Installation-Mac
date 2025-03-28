# Dot-net-Installation-Mac
This guide provides step-by-step instructions to install .NET on macOS using different methods, including Homebrew, the official .NET installer, and Visual Studio for Mac. It also covers post-installation configuration, verification, and uninstallation steps.

# .NET Installation on macOS

This guide provides step-by-step instructions to install .NET on macOS using different methods, including Homebrew, the official .NET installer, and Visual Studio for Mac. It also covers post-installation configuration, verification, and uninstallation steps.

## Method 1: Install Using Homebrew (Recommended)

1. **Open Terminal** (`Cmd + Space`, type "Terminal", and press Enter).
2. **Install Homebrew** (if not installed):
   ```sh
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```
3. **Install .NET SDK**:
   ```sh
   brew install dotnet
   ```
4. **Verify Installation**:
   ```sh
   dotnet --version
   ```

## Method 2: Install Using the Official .NET Installer

1. Go to the official **.NET download page**:  
   👉 [Download .NET](https://dotnet.microsoft.com/en-us/download)
2. Download the latest **.NET SDK** for **macOS**.
3. Open the downloaded `.pkg` file and follow the installation instructions.
4. Verify installation:
   ```sh
   dotnet --version
   ```

## Method 3: Install via Visual Studio for Mac (Optional)

If you are using **Visual Studio for Mac**, it includes .NET by default:

1. Download **Visual Studio for Mac** from:  
   👉 [Visual Studio for Mac](https://visualstudio.microsoft.com/vs/mac/)
2. Install it and follow the setup.
3. Open a new **.NET project**, and it will automatically configure everything.

## Post-Installation Configuration

- **Add .NET to PATH (if necessary)**:
  ```sh
  export PATH="$HOME/.dotnet:$PATH"
  ```
  Add this line to `~/.zshrc` or `~/.bashrc` to persist.

- **Check installed SDKs and Runtimes**:
  ```sh
  dotnet --list-sdks
  dotnet --list-runtimes
  ```

## Uninstall .NET on macOS (If Needed)

If you need to uninstall .NET:
```sh
brew uninstall dotnet
```
Or manually delete it:
```sh
rm -rf /usr/local/share/dotnet
rm -rf ~/.dotnet
```

Let me know if you face any issues! 🚀

---
**Author:** Mohammed Rafi M
**Email:** mhdd24.rafi@gmail.com

