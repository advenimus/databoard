# Changelog

All notable changes to DataBoard will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.0] - 2025-01-17

### Initial Release

DataBoard's first public release brings powerful SQL dashboard capabilities to your desktop.

#### Features

**Database Connectivity**
- SQL Server support with standard and Windows Integrated Authentication
- MySQL/MariaDB connectivity with connection pooling
- PostgreSQL support for versions 10+
- Secure credential storage using OS-level encryption
- Connection testing and validation
- Remote database access via VPN/ZeroTier

**Dashboard & Tile System**
- Drag-and-drop grid layout with 12-column responsive design
- Multiple dashboard support with folder organization
- Configurable auto-refresh intervals per tile
- Save and restore custom layouts
- Dashboard-level parameters for dynamic queries

**Visualizations**
- Line charts with multiple series support
- Bar charts with grouped data
- Pie charts with custom labels
- Interactive data tables with sticky headers
- KPI tiles for key metrics
- Status indicators with color coding
- Gauge visualizations

**Query Management**
- Syntax-highlighted SQL editor with parameter support
- Query history and audit logging
- Connection pooling for optimal performance
- Real-time query execution
- Error handling and validation

**User Interface**
- Modern React-based interface
- Dark/light theme support (coming soon)
- Responsive layout
- Intuitive navigation
- Settings management

**Security & Privacy**
- Passwords encrypted with Electron safeStorage API
- OS-level keychain integration (macOS Keychain, Windows Credential Manager)
- No plain-text credential storage
- Local-first data storage
- No telemetry or usage tracking

**Platform Support**
- macOS ARM64 (Apple Silicon) DMG installer
- Windows x64 NSIS installer (user-level, no admin required)
- Windows x64 portable ZIP archive (no installation needed)
- Ad-hoc code signing for macOS Sequoia compatibility

#### Known Limitations
- Windows ARM64 builds are experimental and not officially supported
- macOS requires manual "Open Anyway" on first launch (unsigned app)
- macOS may require manual Local Network permission grant in System Settings
- Linux builds not included in this release

#### Technical Details
- Built with Electron 33, React 18, TypeScript 5
- Uses better-sqlite3 for local data storage
- Connection drivers: mssql, mysql2, pg
- Cross-platform native module support

---

## Release Notes Format

For future releases, changes will be categorized as:

- **Added** - New features
- **Changed** - Changes in existing functionality
- **Deprecated** - Soon-to-be removed features
- **Removed** - Removed features
- **Fixed** - Bug fixes
- **Security** - Vulnerability fixes

---

[0.1.0]: https://github.com/advenimus/databoard/releases/tag/v0.1.0
