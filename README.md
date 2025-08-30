# My Movies AI - MCP Client

This repository contains the client configuration for the MCP (Model Context Protocol) Movies server.

## Overview

This project uses the Qwen CLI with an MCP server to provide movie information tools. The MCP server runs on a Raspberry Pi 24/7, while this repository contains only the client configuration needed to connect to that server.

## Repository Structure

- **MCP_CLIENT.md** - Documentation for client configuration and usage
- **MCP_SERVER.md** - Documentation for the remote server setup
- **.qwen/settings.json** - MCP server configuration (connects to Raspberry Pi)

## Server Location

The MCP server runs on a Raspberry Pi with the following specifications:
- IP Address: 192.168.0.242
- Port: 3001
- Path: `/home/ay/apps/mcp-movies-server`

## Available Tools

1. **list_movies** - Lists all movies in the database
2. **get_movie_info** - Gets detailed information about a specific movie

## Usage

To use the tools, simply use the Qwen CLI:

```bash
# List all movies
/list_movies

# Get information about a specific movie
/get_movie_info "The Matrix"
```

## Documentation

For detailed information:
- See [MCP_CLIENT.md](MCP_CLIENT.md) for client configuration
- See [MCP_SERVER.md](MCP_SERVER.md) for server setup and management