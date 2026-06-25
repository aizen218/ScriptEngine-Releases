# ScriptEngine

**ScriptEngine** is a modern desktop application for managing isolated browser profiles with per-profile proxy routing. Built with Avalonia UI and .NET 10.

---

## Features

### Profile Management
- Create, edit, duplicate, and delete browser profiles
- Each profile runs in its own isolated `--user-data-dir` with persistent data
- Profiles are stored in a configurable base directory on disk
- Real-time profile status: ready, running, or stopping

### Browser Support
- Detect installed browsers automatically (Chrome, Chromium, Edge, Brave, Opera, Vivaldi)
- Launch any profile with its configured browser
- Runs with `--no-first-run` and `--no-default-browser-check` flags

### Proxy Routing
- Assign a proxy (HTTP, HTTPS, SOCKS4, SOCKS5) to each profile
- Built-in proxy health checker with latency measurement
- Batch import, edit, and delete proxies
- Proxy usage tracking across profiles

### Search & Filter
- Real-time search across profile names, browsers, proxies, and types
- Filterable proxy list with status indicators

### Profiles Folder
- Customizable profiles storage location
- Profile directories are automatically created on first launch, renamed on rename, and cleaned up on deletion

---

## Download

Get the latest release for your platform:

| Platform | Architecture | Format |
|----------|-------------|--------|
| Windows  | x64         | `.zip` |
| Linux    | x64         | `.tar.gz` |

> **Note:** macOS support is planned for a future release.

---

## System Requirements

- **Windows:** Windows 10 1809+ / Windows 11
- **Linux:** .NET 10 compatible distribution (Ubuntu 22.04+, Fedora 38+, etc.)
- **macOS:** *Coming soon*

---

## Quick Start

1. Download the archive for your platform from the [Releases](https://github.com/aizen218/ScriptEngine-Releases/releases) page
2. Extract to a folder of your choice
3. Run `ScriptEngine`

The application will scan for installed browsers and create a local SQLite database on first launch.

---

## Upcoming Features

- **macOS support** – Native builds for Apple Silicon (ARM64) and Intel
- **Workflow automation** – Record and replay browser actions (mouse clicks, form fills, navigation)
- **Profile import/export** – Share profiles across machines
- **Profile groups** – Organize profiles into groups for batch operations
- **Dark/Light theme toggle**
- **Command-line interface** – Launch profiles from terminal

---

## Development

ScriptEngine is built with:

- **Avalonia UI** – Cross-platform desktop framework
- **.NET 10** – Native AOT publishing
- **CommunityToolkit.Mvvm** – MVVM source generators
- **Material.Icons** – Icon set
- **SQLite** – Local data storage

---

## License

MIT
