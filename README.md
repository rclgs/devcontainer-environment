# Dev Container Environment

A comprehensive development container pre-configured with multiple programming languages, tools, and VS Code extensions for full-stack development.

## Overview

This project provides a ready-to-use development environment using VS Code Dev Containers. It includes everything needed for Java, Node.js, and Python development, along with essential development tools and utilities.

## What's Included

### Programming Languages

- **Java 25** (TEM distribution) - Enterprise Java development
- **Node.js 24** - JavaScript/TypeScript runtime for backend and frontend development
- **Python 3.14** - Python scripting and data science

### Development Tools

- **Git** - Pre-installed version control system
- **GitHub CLI** - Command-line interface for GitHub operations
- **npm** - Package manager for Node.js projects
- **pip3** - Package manager for Python projects

### VS Code Extensions

- **ESLint** (`dbaeumer.vscode-eslint`) - JavaScript/TypeScript linting
- **Python** (`ms-python.python`) - Python development support
- **XML** (`redhat.vscode-xml`) - XML editing and validation
- **YAML** (`redhat.vscode-yaml`) - YAML editing and validation
- **Java Language Pack** (`vscjava.vscode-java-pack`) - Comprehensive Java development support

### Base Environment

- Debian GNU/Linux (official Microsoft Dev Containers base image)
- Pre-installed command-line utilities: `curl`, `wget`, `ssh`, `git`, `grep`, `zip`, `tar`, etc.

## Getting Started

### Prerequisites

- VS Code with the Dev Containers extension installed
- Docker installed and running

### Opening the Dev Container

1. Open this folder in VS Code
2. When prompted, click "Reopen in Container" or use the command palette (`Ctrl+Shift+P`) and select "Dev Containers: Reopen in Container"
3. VS Code will build and start the dev container automatically

Once the container is ready, you'll have access to all the pre-installed languages, tools, and extensions.

## Project Structure

```
devcontainer-environment/
├── .devcontainer/
│   └── devcontainer.json    # Dev container configuration
└── README.md                # This file
```

## Configuration

The dev container is configured in `.devcontainer/devcontainer.json`. To customize the environment:

1. Modify the language versions or features in `devcontainer.json`
2. Add or remove VS Code extensions as needed
3. Rebuild the container using "Dev Containers: Rebuild Container"

## Usage Examples

### Java Development

```bash
javac HelloWorld.java
java HelloWorld
```

### Node.js Development

```bash
npm init
npm install package-name
node app.js
```

### Python Development

```bash
python3 -m venv venv
source venv/bin/activate
pip install package-name
python script.py
```

## Additional Features

- **Python Default Interpreter**: Pre-configured to `/usr/local/bin/python` in VS Code
- **Git Integration**: Full git support with GitHub CLI for seamless GitHub workflows
- **Source Control**: Built-in VS Code Git integration for version control within the editor

## Useful Commands

| Command | Purpose |
|---------|---------|
| `git --version` | Check Git version |
| `java -version` | Check Java version |
| `node --version` | Check Node.js version |
| `npm --version` | Check npm version |
| `python3 --version` | Check Python version |
| `gh --version` | Check GitHub CLI version |

## Tips

- All dependencies are pre-installed, so you can start coding immediately
- The container provides an isolated, reproducible development environment
- VS Code automatically syncs your settings within the container
- You can install additional npm packages, pip packages, or use system package managers as needed

## Learn More

- [VS Code Dev Containers Documentation](https://code.visualstudio.com/docs/devcontainers/containers)
- [Dev Containers Specification](https://containers.dev/)
- [Docker Documentation](https://docs.docker.com/)

## License

This dev container configuration is provided as-is for development purposes.
