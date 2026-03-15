# uv-init

An enhanced Python project initialization script based on the `uv` tool that automatically sets up a complete development environment.

## Features

- 🚀 Fast Python project creation using `uv init`
- 📚 Support for library project layout (`--lib` option)
- 🐍 Support for specifying Python version (`--python` option)
- ⚙️ Automatic Ruff configuration (code formatting and linting)
- 📝 Automatic Pyright configuration (type checking)
- 💻 Automatic VS Code settings
- 🎯 One-click complete development environment setup

## Installation

1. Download the script:
```bash
curl -O https://raw.githubusercontent.com/yourusername/uv-init/main/uv-init
```

2. Make it executable:
```bash
chmod +x uv-init
```

3. Move to system path (optional):
```bash
mv uv-init ~/.local/bin/
```

## Usage

### Basic Usage

```bash
# Create a regular Python project
uv-init my-project

# Create a library project
uv-init --lib my-library

# Specify Python version
uv-init --python 3.11 my-project

# Combine options
uv-init --lib --python 3.12 my-awesome-lib
```

### Command Line Options

- `--lib`: Create library project layout (src directory structure)
- `--python <version>`: Specify Python version
- `--help, -h`: Show help information

## Automatic Configurations

### 1. VS Code Configuration (`.vscode/settings.json`)
- Configure Python virtual environment path
- Enable format on save
- Set Ruff as default formatter
- Configure auto-organize imports and fix issues on save

### 2. Pyright Configuration (`pyrightconfig.json`)
- Set Python version
- Standard type checking mode
- Optimized error reporting configuration

### 3. Ruff Configuration (appended to `pyproject.toml`)
- Code line length limit: 88 characters
- Target Python version: auto-detect
- Comprehensive code checking rules
- Auto-fix all fixable issues

## Examples

Create a project named `my-app`:

```bash
uv-init my-app
cd my-app
```

This creates:
- Complete Python project structure
- Configured development environment
- Ready-to-code environment

## Requirements

- [uv](https://github.com/astral-sh/uv): Python package management tool
- Python 3.8+ (3.11+ recommended)

## License

MIT License - see [LICENSE](LICENSE) file for details

## Contributing

Issues and Pull Requests are welcome!

## Why choose this script?

The standard `uv init` only creates basic project structure. This script adds:

1. **Out of the box**: No manual development environment setup needed
2. **Best practices**: Pre-configured with modern Python development best practices
3. **Tool integration**: Perfect integration with VS Code, Ruff, Pyright
4. **Flexible configuration**: Support for different project types and Python versions

Focus on coding, not environment configuration!

---

**Language:** English | [中文](README.zh.md)
