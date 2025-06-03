
# BrightDataMCPServerAgent

## Description
BrightDataMCPServerAgent is a Python template project for building an MCP (Model Context Protocol) server agent using LangChain, Anthropic, and Bright Data MCP adapters. It provides a starting point for integrating language models and toolchains with the MCP protocol, supporting advanced agent workflows and tool use.



## Features
- Integrates LangChain and Anthropic Claude models for advanced LLM reasoning.
- Grants agents real-time web search, data extraction, and automation via Bright Data MCP tools (mainly for web scraping and browser automation).
- Enables multi-step tool use and web workflows in a single agent.
- Secure environment variable management with `.env`.

## Agent Capabilities
- Search and extract web data in real time.
- Chain tool calls and automate browser actions.
- Combine LLM reasoning (Anthropic Claude) with external tool use.


## About Bright Data & Anthropic
- **Bright Data MCP**: Enables agents to access, search, and extract web data at scale. [Bright Data Website](https://brightdata.com/products/mcp) — [Get your Bright Data API key](https://brightdata.com/console/settings/tokens)
- **Anthropic Claude**: Provides advanced language understanding and planning for agent workflows. [Anthropic Website](https://www.anthropic.com/) — [Get your Anthropic API key](https://console.anthropic.com/settings/keys)

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



## About `uv` and Common Commands
[`uv`](https://github.com/astral-sh/uv) is a fast Python package manager and build tool. Common commands used in this project:
- `uv pip install -r pyproject.toml` — Installs all dependencies listed in `pyproject.toml`.
- `uv pip install <package>` — Installs an individual package.
- `uv run main.py` — Runs your main Python script in the current environment.


## Usage Example
To start the agent, run:
```sh
uv run main.py
```
You can then interact with the agent in your terminal.

## Example .env File
Create a `.env` file in your project root with the following content:
```env
API_TOKEN=your-brightdata-api-token
BROWSER_AUTH=your-browser-auth
WEB_UNLOCKER_ZONE=your-web-unlocker-zone
ANTHROPIC_API_KEY=your-anthropic-api-key
```

## Troubleshooting
- **Anthropic API credit error:** If you see the message `Your credit balance is too low to access the Anthropic API. Please go to Plans & Billing to upgrade or purchase credits.`, add credits to your Anthropic account or use a different API key with an active balance.
- **Missing environment variables:** Ensure your `.env` file is present and all required variables are set.


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
Specify your license here (e.g., MIT, Apache 2.0, etc.).


## References
Much of the information and setup in this project was based on the following YouTube video:
[Bright Data MCP Server Agent Tutorial](https://www.youtube.com/watch?v=6DXuadyaJ4g)

## Contributing
Pull requests and issues are welcome!

