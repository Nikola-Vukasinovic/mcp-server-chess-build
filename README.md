# MCP Server Chess Build

This repository contains an MCP server for Chess.com, built using the [mcp](https://github.com/modelcontext/mcp) framework.

## Installation

1. **Clone the repository:**
   ```powershell
   git clone <this-repo-url>
   cd mcp-server-chess-build
   ```


2. **Install [uv](https://github.com/astral-sh/uv) (if not already installed):**
   - **uv is a standalone tool.** Download and install it from the official site:
     https://docs.astral.sh/uv/guides/projects/

   - **On Windows:**
     Download the latest Windows release from the [uv releases page](https://github.com/astral-sh/uv/releases), extract the executable, and add it to your PATH.

   - **On Linux/macOS:**
     Download the appropriate binary from the [uv releases page](https://github.com/astral-sh/uv/releases), extract it, and add it to your PATH.

   - See the [official uv installation guide](https://docs.astral.sh/uv/guides/projects/) for detailed instructions for your platform.

3. **Install dependencies and the package:**
   - **On Windows:**
     ```powershell
     uv pip install -e .
     ```
   - **On Linux/macOS:**
     ```bash
     uv pip install -e .
     ```

*This will install all dependencies in editable (development) mode.*

**Note:** All paths and commands in this README are shown for Windows (PowerShell). If you are using Linux or macOS, adjust paths and commands accordingly (e.g., use `/` instead of `\`, and use `source .venv/bin/activate` to activate a virtual environment).* 

## Usage


You can run the MCP server using the installed script:

```powershell
chess
```

Or directly with Python:

```powershell
python -m chess.server
```

The server will start and listen for MCP requests via stdio.

## Requirements
- Python 3.13 or higher
- [uv](https://github.com/astral-sh/uv)

## Development

To install in editable mode (already covered above):
```powershell
uv pip install -e .
```

## Testing

To run tests (if you have any):
```powershell
uv pip install pytest
pytest
```

## Using VS Code Agent

You can use the VS Code agent (such as GitHub Copilot or other AI coding assistants) to add, configure, and test your MCP server directly in a VS Code host environment:

1. **Open the project in VS Code:**
   - Use `File > Open Folder...` and select your `mcp-server-chess-build` directory.

2. **Install recommended extensions:**
   - For Python development, install the "Python" extension by Microsoft.
   - For uv support, you may use the "uv" extension if available, or run uv commands in the integrated terminal.
   - For AI assistance, install "GitHub Copilot" or your preferred agent.

3. **Set up your environment:**
   - Open a terminal in VS Code (`Terminal > New Terminal`).
   - Run the installation steps above using uv.

4. **Run and test the server:**
   - Use the terminal to run `chess` or `python -m chess.server`.
   - Use the VS Code testing UI or terminal to run `pytest` for your tests.

5. **Use the agent:**
   - Ask the agent to add features, write tests, or refactor code. For example, type a request in the chat panel or use inline suggestions.

This workflow allows you to develop, test, and extend your MCP server efficiently within VS Code using modern tools and AI assistance.

**Note:**
On some hosts, you can use `npx` to run certain agents or tools without needing to download or install them globally. For example:

```powershell
npx <agent-or-tool>
```
This can be useful for quickly trying out agents or utilities in your VS Code environment without additional setup.

---

### Linux/macOS Quick Start

1. Open a terminal and clone the repository:
   ```bash
   git clone <this-repo-url>
   cd mcp-server-chess-build
   ```
2. Install uv and dependencies:
   ```bash
   pip install uv
   uv pip install -e .
   ```
3. Run the server:
   ```bash
   chess
   # or
   python -m chess.server
   ```
