# School Fee Manager Desktop - v3.0.0

Complete desktop application for managing school fees with offline SQLite database storage.

## 🚀 Quick Start

### Prerequisites
- Node.js 22+ (REQUIRED for Vite 7)
- npm or yarn

### Installation

```bash
# Install dependencies
npm install

# Development mode
npm run dev

# Build for production
npm run build

# Run Electron app in development
npm run electron:dev

# Build Electron app
npm run electron:build:win   # For Windows
npm run electron:build:mac   # For macOS
npm run electron:build:linux # For Linux
```

## 📦 Project Structure

```
school-fee-manager-desktop/
├── src/                    # React source code
├── electron/              # Electron main process
├── assets/                # Icons and resources
├── dist/                  # Web build output
├── release/               # Electron build output
├── package.json           # Dependencies (with "type": "module")
├── vite.config.ts         # Vite configuration
├── tsconfig.json          # TypeScript configuration
└── appveyor.yml          # CI/CD configuration
```

## 🔧 Technologies Used

- **Frontend**: React 19, TypeScript, Tailwind CSS 4
- **Build Tool**: Vite 7
- **Desktop**: Electron 28
- **Database**: SQLite3
- **Charts**: Recharts
- **Icons**: Lucide React

## 📝 Important Configuration

### package.json
- ✅ `"type": "module"` - Enables ES modules (REQUIRED)
- ✅ `vite: "^7.2.0"` - Latest Vite version
- ✅ `vite-plugin-singlefile` - Single file builds

### appveyor.yml
- ✅ Node.js 22+ - Required for Vite 7
- ✅ Automated builds on push
- ✅ Artifacts generation

## 🎯 Build Output

- **Web Build**: `dist/` folder - Single HTML file with embedded assets
- **Desktop Build**: `release/` folder - Platform-specific installers

## 🐛 Troubleshooting

### Build Fails with "ERR_REQUIRE_ESM"
✅ **Fixed**: `"type": "module"` added to package.json

### Build Fails with Node.js Version Error
✅ **Fixed**: AppVeyor uses Node.js 22+

### "Cannot find path specified" Error
✅ **Fixed**: AppVeyor config updated for root-level project

## 📄 License

Commercial - © 2026 MWA Software

## 🆘 Support

For issues or questions, contact MWA Software support.

---

**Status**: ✅ Ready for GitHub deployment
**Last Updated**: February 15, 2026
