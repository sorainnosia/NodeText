

https://github.com/user-attachments/assets/87494ce1-ab30-4019-9a79-6f4e5f6a586f

# NodeText

A lightweight, blazing-fast code editor with built-in Rust debugging via GDB/LLDB. Built with Rust and Tauri for Windows and Android.

**Website:** [https://nodetext.org](https://nodetext.org) | **Documentation:** [https://nodetext.org/Documentation](https://nodetext.org/Documentation)

## Features
https://github.com/user-attachments/assets/9f1a487d-b59f-42f0-845b-f6ef17cd6d9d

### Syntax Highlighting
- **30+ languages** — Rust, JavaScript, TypeScript, Python, C, C++, C#, Java, Go, HTML, CSS, JSON, XML, SQL, Markdown, TOML, YAML, Shell/Bash, Batch, PowerShell, Ruby, PHP, Kotlin, Swift, Dart, Lua, R, Perl, Scala, Zig, Elixir, Haskell, GraphQL, Protobuf, Dockerfile, Razor/CSHTML, ASPX, CSV
- Viewport-based rendering for large files with zero lag
- Auto language detection from file extension and content analysis
- Manual language selection via toolbar dropdown

### Code Editing
- **Auto-indent** — language-aware indentation on Enter, with Rust-specific rules for match arms, where clauses, and method chains
- **Bracket matching** — highlights matching `{}`, `[]`, `()` pairs, plus HTML/XML tag matching and generic angle brackets
- **Auto-close brackets** — wraps selected text with bracket/quote pairs automatically
- **Code folding** — AST-based folding for Rust, brace-based for other languages; click gutter markers to collapse/expand
- **Block selection** — Alt+Shift+Drag for rectangular/column selection with copy and delete support
- **Code completion** — context-aware autocomplete for language keywords, Rust standard library methods, struct fields (after `.`), module items (after `::`), file/project symbols, and buffer words
- **Hover information** — type hints on hover for Rust symbols
- **Document formatting** — Ctrl+K, D to pretty-format JSON and XML/HTML files
- **Comment/Uncomment** — Ctrl+K, C to comment and Ctrl+K, U to uncomment selected lines, with language-appropriate comment syntax
- **Line numbers** with current line highlighting
- **Word wrap** toggle (Alt+Z or toolbar button)
- **Smart Home key** — toggles between first non-whitespace and column 0

### Find & Replace
- **Ctrl+F** — find with real-time match highlighting (yellow for current match, orange for others)
- **Ctrl+H** — find and replace with Replace and Replace All
- **F3 / Shift+F3** — navigate to next/previous match
- **Ctrl+Shift+F** — search across all files in the open project

### Navigation
- **File tabs** — multiple open files with tab switching (Ctrl+Tab / Ctrl+Shift+Tab), drag to reorder, modified indicator
- **File explorer** — folder tree with filter bar, right-click context menu (New File, New Folder, Rename, Delete, Copy, Cut, Paste)
- **Outline** — code symbols (functions, structs, etc.) for the current file in the explorer panel
- **Breadcrumb bar** — shows the current scope hierarchy, clickable to jump to scope locations
- **Go to Line** — Ctrl+G to jump to a specific line number
- **Go to Definition** — F12 or Ctrl+Click to jump to symbol definition, searches local project files and path-based crate dependencies
- **Error navigation** — F8 / Shift+F8 to cycle through cargo check errors with red underlines and hover messages

### Rust Debugging via GDB/LLDB
- **Breakpoints** — click the gutter to set breakpoints with conditional expressions and thread ID filtering
- **Step controls** — Step In (F11), Step Over (F10), Step Out (Shift+F11), Continue (F5), Stop (Shift+F5) with macro-aware stepping
- **Watch & Locals** — inspect local variables, add watch expressions, expand nested structs, view String contents, Vec lengths; smart type simplification (e.g., `alloc::string::String` shown as `String`); automatic Box/Rc/Arc unwrapping
- **MSVC PDB support** — debug Rust programs compiled with the MSVC toolchain on Windows
- **Auto LLVM install** — automatically downloads and installs LLVM with a progress dialog if no debugger is found
- **Build & diagnostics** — Ctrl+Shift+B to run cargo build with inline error underlines

### Integrated Terminal
- Built-in shell panel (Ctrl+\`) for running cargo, git, and other commands
- Command history navigation (Arrow Up/Down)
- Interrupt support (Ctrl+Shift+C)
- Syntax-colored cargo check output

### Themes & Appearance
- **Dark theme** — Catppuccin Mocha (default)
- **Light theme** — Catppuccin Latte
- **Font stack** — Cascadia Code, Fira Code, JetBrains Mono, Consolas, monospace
- **Font size** — configurable 10px-24px, adjustable with Ctrl+Mouse Wheel
- Theme and font settings sync across pop-out windows

### Panels & Windows
- **Pop-out windows** — detach File Explorer, Debug/Watch, Search Results, Terminal, and Chart panels into separate windows
- **Resizable panels** — drag borders to resize explorer, watch panel, terminal, and search results
- **Claude AI panel** — integrated AI assistant (requires Anthropic API key)
- **Chart visualization** — interactive graphs for Rust code structure, call graphs, dependency maps, module layout, type hierarchy, and complexity heatmaps

### Custom Shortcuts
- Add keyboard shortcuts that execute terminal commands via Settings > Shortcuts
- Map any Ctrl/Alt/Shift + key combination to a command
- Built-in shortcuts are protected from override

### Other
- **Drag & drop** — drop files from the system file manager to open them
- **Session restore** — auto-saves and restores open tabs, scroll position, and cursor position
- **Status bar** — cursor position, language, encoding (UTF-8), build/debug status

### Cross Platform
- **Windows** — native app with WebView2, full GDB/LLDB debugging with MSVC PDB
- **Android** — touch-optimized with slide-in file explorer, adaptive toolbar, and native file picker

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
| **Debugging** | GDB/LLDB (auto-downloaded) | — |

## Keyboard Shortcuts

### File Operations

| Shortcut | Action |
|---|---|
| Ctrl+O | Open file |
| Ctrl+S | Save |
| Ctrl+Shift+S | Save As |
| Ctrl+N | New file |
| Ctrl+W | Close current tab |

### Editing

| Shortcut | Action |
|---|---|
| Ctrl+Z | Undo |
| Ctrl+Y / Ctrl+Shift+Z | Redo |
| Ctrl+A | Select all |
| Ctrl+C / X / V | Copy / Cut / Paste |
| Tab | Insert tab / Indent selection |
| Shift+Tab | Dedent selection |
| Home | Smart home (first non-whitespace / column 0) |
| Alt+Z | Toggle word wrap |
| Alt+Arrow Up/Down | Move line up/down (expand/shrink scope in Rust) |
| Alt+Shift+Drag | Block (column) selection |
| Ctrl+Mouse Wheel | Adjust font size |

### Chord Shortcuts (Ctrl+K, then...)

| Shortcut | Action |
|---|---|
| Ctrl+K, D | Format document (JSON, XML, HTML) |
| Ctrl+K, C | Comment selection |
| Ctrl+K, U | Uncomment selection |

### Find & Replace

| Shortcut | Action |
|---|---|
| Ctrl+F | Find |
| Ctrl+H | Find & Replace |
| F3 / Shift+F3 | Next / Previous match |
| Ctrl+Shift+F | Find in project |
| Escape | Close find bar |

### Navigation

| Shortcut | Action |
|---|---|
| Ctrl+G | Go to line |
| F12 / Ctrl+Click | Go to definition |
| Ctrl+Tab | Next tab |
| Ctrl+Shift+Tab | Previous tab |
| F8 / Shift+F8 | Next / Previous error |

### Debugging

| Shortcut | Action |
|---|---|
| F5 | Start / Continue |
| Shift+F5 | Stop debugging |
| F9 | Toggle breakpoint |
| F10 | Step Over |
| F11 | Step Into |
| Shift+F11 | Step Out |
| Ctrl+Shift+B | Build project |

### Terminal

| Shortcut | Action |
|---|---|
| Ctrl+\` | Toggle terminal |
| Ctrl+Shift+C | Send interrupt |
| Arrow Up/Down | Command history |

## Built With

- [Rust](https://www.rust-lang.org/) — Backend
- [Tauri v2](https://tauri.app/) — Native app framework
- [GDB](https://sourceware.org/gdb/) / [LLDB](https://lldb.llvm.org/) — Debugger engines

## License

Copyright 2025 NodeText. All rights reserved.
