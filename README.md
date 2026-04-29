# NodeText

A lightweight, blazing-fast code editor with built-in Rust debugging via LLDB. Built with Rust and Tauri for Windows and Android.

**Website:** [https://nodetext.org](https://nodetext.org)

## Features
https://github.com/user-attachments/assets/e9235f32-0de1-4595-8ddc-892bc06a38c6


### Rust Debugging via LLDB
- **Breakpoints** — Click the gutter to set breakpoints with conditional expressions and thread ID filtering
- **Step Controls** — Step In, Step Over, Step Out, Continue, and Pause with macro-aware stepping
- **Watch & Locals** — Inspect local variables, add watch expressions, view String contents, Vec lengths, and nested struct fields
- **MSVC PDB Support** — Debug Rust programs compiled with the MSVC toolchain on Windows
- **Auto LLVM Install** — Automatically downloads and installs LLVM with a progress dialog if no debugger is found

### Integrated Terminal
- Built-in shell panel (Ctrl+`) for running cargo, git, and other commands
- ANSI color support in terminal output

### Syntax Highlighting
- 20+ languages: Rust, Python, JavaScript, TypeScript, C/C++, C#, Java, Go, HTML, CSS, JSON, XML, TOML, Markdown, Shell/Bash, Batch, CSV, INI, Log files, Razor/CSHTML
- Viewport-based rendering for large files with zero lag
- Auto language detection from file extension

### Find & Replace
- Ctrl+F to find with real-time match highlighting (orange for current match, blue for others)
- Ctrl+H for find and replace with Replace All
- Enter/F3 navigates to next match while keeping focus in the search input

### Editor
- Line numbers with current line highlighting
- Word wrap toggle
- Multiple file buffers with tabs
- File explorer with right-click context menu (Rename, Delete, Cut, Copy, Paste)
- Resizable panels — drag borders to resize explorer, watch panel, and terminal
- Project-wide search

### Cross Platform
- **Windows** — Native app with WebView2, full LLDB debugging with MSVC PDB
- **Android** — Touch-optimized with slide-in file explorer, adaptive toolbar, and native file picker

## Download

- **Windows:** [nodetext.exe](https://github.com/sorainnosia/NodeText/releases)
- **Android:** [Google Play Store](https://play.google.com/store/apps/details?id=com.nodetext.editor)

## System Requirements

| | Windows | Android |
|---|---|---|
| **OS** | Windows 10+ (64-bit) | Android 7.0+ (API 24) |
| **RAM** | 128 MB | 64 MB |
| **Size** | ~20 MB | ~10 MB |
| **Runtime** | WebView2 | Android System WebView |
| **Debugging** | LLVM/LLDB (auto-downloaded) | — |

## Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| Ctrl+O | Open file |
| Ctrl+S | Save |
| Ctrl+Shift+S | Save As |
| Ctrl+F | Find (toggle) |
| Ctrl+H | Find & Replace (toggle) |
| Ctrl+Shift+F | Search in project |
| F3 | Find next |
| Ctrl+` | Toggle terminal |
| F5 | Start debugging |
| F9 | Toggle breakpoint |
| F10 | Step Over |
| F11 | Step In |
| Shift+F11 | Step Out |
| F6 | Continue |
| Ctrl+C/X/V | Copy/Cut/Paste (also works in file explorer) |

## Built With

- [Rust](https://www.rust-lang.org/) — Backend
- [Tauri v2](https://tauri.app/) — Native app framework
- [LLDB](https://lldb.llvm.org/) — Debugger engine

## License

Copyright 2025 NodeText. All rights reserved.
