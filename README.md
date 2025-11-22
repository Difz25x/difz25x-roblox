# DIFZ25X DOWNGRADER

![Version](https://img.shields.io/badge/version-1.0.0-black?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-white?style=flat-square)
![Platform](https://img.shields.io/badge/platform-Windows-lightgrey?style=flat-square)

> **A modern terminal-style Roblox version downgrader with multi-instance support**

---

## 📋 Table of Contents

- [Features](#-features)
- [Prerequisites](#-prerequisites)
- [Installation](#-installation)
- [Usage](#-usage)
- [Configuration](#-configuration)
- [Building](#-building)
- [Troubleshooting](#-troubleshooting)
- [Contributing](#-contributing)
- [License](#-license)

---

## ✨ Features

- **🎯 Version Selection** - Choose from 3 pre-configured Roblox versions
- **⚡ Auto Download** - Automated download and extraction process
- **🚀 Multi-Instance** - Launch multiple Roblox instances simultaneously
- **📊 Real-time Progress** - Live download progress tracking
- **💾 Smart Caching** - Downloads once, reuse multiple times
- **🖥️ Terminal UI** - Clean black & white interface with scanline effects
- **🔄 Instance Tracking** - Monitor active Roblox instances
- **⚙️ Auto-Updates** - Built-in update checker (optional)

---

## 📦 Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (v16.0.0 or higher)
- **npm** (v7.0.0 or higher)
- **Windows OS** (Windows 10/11)

---

## 🔧 Installation

### Method 1: From Source

```bash
# Clone the repository
git clone https://github.com/Difz25x/difz25x-downgrader.git

# Navigate to project directory
cd difz25x-downgrader

# Install dependencies
npm install

# Run the application
npm start
```

### Method 2: Pre-built Release

1. Download the latest release from [Releases](https://github.com/yourusername/difz25x-downgrader/releases)
2. Extract the ZIP file
3. Run `Difz25x-Downgrader.exe`

---

## 🎮 Usage

### Basic Workflow

1. **Launch Application**
   ```bash
   npm start
   ```

2. **Select Version**
   - Choose from 3 available Roblox versions
   - See installation status ([READY] or [NEW])

3. **Download & Launch**
   - Click `[ Download & Launch ]` for new versions
   - Click `[ Launch ]` for installed versions

4. **Multi-Instance**
   - After first launch, use `[ Launch More ]` button
   - Track active instances in the UI

### Version Management

The downgrader supports 3 pre-configured versions:

- **Version 1**: `version-8e6e698468a04d3f`
- **Version 2**: `version-fdda949d95e447e3`
- **Version 3**: `version-e380c8edc8f6477c`

All versions are cached locally after first download.

---

## ⚙️ Configuration

### Adding New Versions

Edit `main.js` and modify the `AVAILABLE_VERSIONS` array:

```javascript
const AVAILABLE_VERSIONS = [
    { id: 'version1', name: 'Version 1', hash: 'version-8e6e698468a04d3f' },
    { id: 'version2', name: 'Version 2', hash: 'version-fdda949d95e447e3' },
    { id: 'version3', name: 'Version 3', hash: 'version-e380c8edc8f6477c' },
];
```

### File Locations

- **Downloads**: `%APPDATA%/difz25x-downgrader/downloads/`
- **Installed Versions**: `%APPDATA%/difz25x-downgrader/versions/`
- **Logs**: Console output (press F12 in dev mode)

---

## 🔨 Building

### Development Build

```bash
# Run in development mode
npm start

# Run with dev tools
npm run dev
```

### Production Build

```bash
# Build for Windows
npm run build

# Build for Windows (x64)
npm run build:win

# Build and create installer
npm run dist

---

## 🐛 Troubleshooting

### Common Issues

#### Application won't start
```bash
# Clear cache and reinstall
rm -rf node_modules
npm install
npm start
```

#### Download fails
- Check internet connection
- Ensure firewall allows the application
- Try different Roblox version
- Check antivirus settings

#### Roblox won't launch
- Verify version is fully downloaded
- Check if file size is > 1MB
- Try re-downloading the version
- Run as administrator

#### Multiple instances not working
- Ensure first instance is fully loaded
- Wait 2-3 seconds between launches
- Check Task Manager for zombie processes

### Debug Mode

Press `F12` to open Developer Tools and check console logs.

---

## 📊 System Requirements

| Component | Minimum | Recommended |
|-----------|---------|-------------|
| OS | Windows 10 | Windows 11 |
| RAM | 4GB | 8GB+ |
| Storage | 500MB | 2GB+ |
| Internet | Required | Broadband |
| CPU | Dual-core | Quad-core+ |

---

## 🔐 Security

- All downloads are from official Roblox CDN
- No data collection or telemetry
- Open source - audit the code yourself
- Local storage only (no cloud sync)

---

## 🤝 Contributing

Contributions are welcome! Here's how:

1. Fork the repository
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request

### Development Guidelines

- Follow existing code style
- Test all changes thoroughly
- Update documentation as needed
- Keep commits atomic and descriptive

---

## 📝 Changelog

### Version 1.0.0 (2025-01-XX)
- Initial release
- Version selection system
- Multi-instance support
- Terminal-style UI
- Auto-download functionality
- Progress tracking
- Instance monitoring

---

## 🙏 Credits

**Developed by Difz25x**
- UI Design: Terminal/Cyberpunk aesthetic
- Core Logic: Electron + Puppeteer
- Community: Difz25x Community

### Dependencies

- [Electron](https://www.electronjs.org/) - Desktop framework
- [Puppeteer Real Browser](https://github.com/zfcsoftware/puppeteer-real-browser) - Browser automation
- [AdmZip](https://github.com/cthackers/adm-zip) - ZIP extraction
- [Node.js](https://nodejs.org/) - Runtime environment

---

## 📄 License

This project is licensed under the MIT License - see below for details:

```
MIT License

Copyright (c) 2025 Difz25x Community

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/yourusername/difz25x-downgrader/issues)
- **Discussions**: [GitHub Discussions](https://github.com/yourusername/difz25x-downgrader/discussions)
- **Discord**: [Join our server](#) (optional)

---

## ⚠️ Disclaimer

This tool is for educational purposes only. Use at your own risk. The developers are not responsible for any misuse or damage caused by this software.

---

<div align="center">

**Made with ❤️ by Difz25x Community**

[⬆ Back to Top](#difz25x-downgrader)

</div>
