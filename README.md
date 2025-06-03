
# BrightDataMCPServerAgent

## Description
BrightDataMCPServerAgent is a Python template project for building an MCP (Model Context Protocol) server agent using LangChain, Anthropic, and Bright Data MCP adapters. It provides a starting point for integrating language models and toolchains with the MCP protocol, supporting advanced agent workflows and tool use.


## Features
- Integrates LangChain and Anthropic Claude models for advanced LLM reasoning.
- Grants agents real-time web search, data extraction, and automation via Bright Data MCP tools.
- Enables multi-step tool use and web workflows in a single agent.
- Secure environment variable management with `.env`.

## Agent Capabilities
- Search and extract web data in real time.
- Chain tool calls and automate browser actions.
- Combine LLM reasoning (Anthropic Claude) with external tool use.

## About Bright Data & Anthropic
- **Bright Data MCP**: Enables agents to access, search, and extract web data at scale.
- **Anthropic Claude**: Provides advanced language understanding and planning for agent workflows.

## Requirements
- Python >= 3.13
- See dependencies in `pyproject.toml` or `uv.lock`

## Installation
1. Clone the repository:
   ```sh
   git clone <your-repo-url>
   cd mcp_template_anthropic
   ```
2. Create and activate a virtual environment:
   ```sh
   python3 -m venv .venv
   source .venv/bin/activate
   ```
3. Install dependencies:
   ```sh
   uv pip install -r pyproject.toml
   ```

## Usage
1. Set up your `.env` file with the required environment variables:
   - `API_TOKEN`
   - `BROWSER_AUTH`
   - `WEB_UNLOCKER_ZONE`
2. Run the main agent:
   ```sh
   uv run main.py
   ```

## Project Structure
- `main.py` — Example entry point for the MCP agent
- `mcp_template/` — Your package code
- `pyproject.toml` — Project metadata and dependencies
- `uv.lock` — Locked dependency versions

## Changes
- Initial template setup
- Added LangChain, Anthropic, and MCP adapters
- Example async agent in `main.py`

## License
Add your license here.

## Contributing
Pull requests and issues are welcome!

