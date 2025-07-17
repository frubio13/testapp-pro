# TestApp Pro - Sistema de Oposiciones

## Overview
TestApp Pro is a React-based Electron application designed for managing educational tests and examinations, specifically tailored for Spanish opposition exam preparation. The application combines web and desktop capabilities, providing a comprehensive testing platform with AI integration and secure local storage.

## Project Structure

### Core Files
- **`index.html`** - Entry point for the React application (704 bytes)
- **`main.js`** - Full-featured Electron main process with comprehensive menu system (304 lines)
- **`electron.js`** - Simplified Electron main process (58 lines)
- **`asset-manifest.json`** - Build manifest mapping source files to hashed filenames

### Static Assets
```
static/
├── css/
│   ├── main.963b8657.css (1.3KB)
│   └── main.963b8657.css.map (2.7KB)
├── js/
│   ├── main.48711daa.js (487KB)
│   ├── main.48711daa.js.map (2.9MB)
│   ├── 453.e8d38cfc.chunk.js (4.4KB)
│   ├── 453.e8d38cfc.chunk.js.map (11KB)
│   └── main.48711daa.js.LICENSE.txt (8.7KB)
└── media/
    └── imagen.32091d55a91ae26a5d06.jpg (317KB)
```

### Media Files
- **`imagen.jpg`** - Original background image (324KB)
- **`favicon.ico`** - Application icon (3.8KB)

## Technical Stack

### Framework & Technologies
- **Frontend**: React.js (Create React App)
- **Desktop**: Electron
- **Build**: Production-optimized with webpack
- **Deployment**: GitHub Pages (gh-pages branch)

### Application Configuration
- **Window Size**: 1400x900 (minimum: 1000x700)
- **Node Integration**: Enabled
- **Context Isolation**: Disabled
- **Web Security**: Disabled (for local file access)
- **Development Port**: http://localhost:3000

## Features

### Core Functionality
1. **Test Management System**
   - Create new tests
   - Quick test mode
   - Exam simulation
   - Statistics tracking

2. **Data Management**
   - Import/export questions (TXT, JSON formats)
   - Local data storage in user directory
   - Question sharing capabilities
   - Secure local storage

3. **User Interface Features**
   - Modern card-based design
   - Responsive layout
   - Full-screen mode
   - Zoom controls (in/out/reset)
   - Development tools access

### Menu System

#### File Menu
- **New Test** (`Ctrl+N`)
- **Open Data Folder** (`Ctrl+O`)
- **Export Questions** (`Ctrl+E`)
- **Import Questions** (`Ctrl+I`)

#### Test Menu
- **Quick Test** (`Ctrl+T`)
- **Exam Simulation** (`Ctrl+Shift+T`)
- **Show Statistics** (`Ctrl+S`)

#### View Menu
- **Reload** (`Ctrl+R`)
- **Force Reload** (`Ctrl+Shift+R`)
- **Zoom In** (`Ctrl++`)
- **Zoom Out** (`Ctrl+-`)
- **Reset Zoom** (`Ctrl+0`)
- **Full Screen** (`F11`)
- **Developer Tools** (`F12`)

#### Help Menu
- **Keyboard Shortcuts**
- **About TestApp Pro**

## Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl+N` | New Test |
| `Ctrl+T` | Quick Test |
| `Ctrl+Shift+T` | Exam Simulation |
| `Ctrl+S` | Show Statistics |
| `Ctrl+E` | Export Questions |
| `Ctrl+I` | Import Questions |
| `Ctrl+O` | Open Data Folder |
| `Ctrl+R` | Reload |
| `Ctrl+Shift+R` | Force Reload |
| `Ctrl++` | Zoom In |
| `Ctrl+-` | Zoom Out |
| `Ctrl+0` | Reset Zoom |
| `F11` | Full Screen |
| `F12` | Developer Tools |

## Design & Styling

### Visual Design
- **Background**: Full-screen background image with cover sizing
- **Layout**: Card-based design with rounded corners (12px border-radius)
- **Colors**: Material Design inspired color scheme
  - Primary: Blue (#1976d2)
  - Response options: Red (#e53935), Blue (#1e88e5), Green (#43a047), Orange (#fb8c00)
- **Typography**: System fonts with fallbacks
- **Shadows**: Subtle box shadows for depth

### Response Styling
- **Option A**: Red (#e53935) - Bold
- **Option B**: Blue (#1e88e5) - Bold
- **Option C**: Green (#43a047) - Bold
- **Option D**: Orange (#fb8c00) - Bold

### Responsive Design
- Mobile-friendly with media queries
- Adjustable button sizes for smaller screens
- Flexible layout system

## Development vs Production

### Development Mode
- Loads from `http://localhost:3000`
- Auto-opens Developer Tools
- Hot reload enabled

### Production Mode
- Loads from `file://../build/index.html`
- Minified and optimized assets
- Source maps available for debugging

## Repository Information

### Git Configuration
- **Repository**: testapp-pro
- **Owner**: frubio13
- **Current Branch**: gh-pages
- **Default Branch**: gh-pages

### Remote Repositories
- **Origin**: `git@github.com:frubio13/testapp-pro.git`
- **Upstream**: `git@github.com:HitZZie/testapp-pro.git`

### Status
- Clean working tree
- Up to date with origin/gh-pages

## Build Information

### Optimization
- **Minified**: All JavaScript and CSS files are minified
- **Compressed**: Gzipped for optimal loading
- **Cache-busting**: Content hashes in filenames
- **Source Maps**: Available for debugging

### License Information
- Includes Google/Apache license compliance
- Third-party licenses documented in LICENSE.txt

## File Paths & URLs

### Asset Paths
All assets are served with the `/testapp-pro/` prefix for GitHub Pages deployment:
- CSS: `/testapp-pro/static/css/main.963b8657.css`
- JavaScript: `/testapp-pro/static/js/main.48711daa.js`
- Media: `/testapp-pro/static/media/imagen.32091d55a91ae26a5d06.jpg`

### Entry Points
- **CSS**: `static/css/main.963b8657.css`
- **JavaScript**: `static/js/main.48711daa.js`

## IPC Communication

### Available Handlers
- **show-save-dialog**: File save dialog
- **show-open-dialog**: File open dialog
- **get-app-path**: Application path retrieval
- **show-item-in-folder**: Open file location in system explorer

### Event Listeners
- **new-test**: Create new test
- **start-quick-test**: Start quick test mode
- **start-exam-simulation**: Start exam simulation
- **show-statistics**: Display statistics
- **export-questions**: Export questions
- **import-questions**: Import questions
- **open-settings**: Open settings panel

## Security Features

### Local Storage
- Secure local data storage in user directory
- No external data transmission
- Private file access for user data

### File System Access
- Local file import/export capabilities
- System dialog integration
- Secure file handling

## Error Handling

### Process Error Management
- Uncaught exception handling
- Unhandled promise rejection handling
- Graceful error recovery

## Deployment

### GitHub Pages
- Deployed on gh-pages branch
- Static asset hosting
- Automatic deployment pipeline

### Electron Distribution
- Cross-platform desktop application
- Native system integration
- Offline functionality

## Usage Modes

### Web Application
- Accessible via GitHub Pages
- Browser-based interface
- Limited file system access

### Desktop Application
- Full Electron functionality
- Complete file system access
- Native menu integration
- System notifications

## Development Notes

### Missing Development Files
This appears to be a production deployment with the following development files absent:
- `package.json` (dependency management)
- Source code files
- Development configuration
- README documentation

### Build Process
- Created with Create React App
- Webpack bundling
- Production optimization
- Asset hashing for cache management

---

*Last updated: July 17, 2025*
*Repository: frubio13/testapp-pro*
