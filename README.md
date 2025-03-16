# MCP Calculator Tool

A simple calculator tool implemented using the Model Context Protocol (MCP).

## Features

- Performs basic arithmetic addition
- Integrated with Cursor IDE
- Type-safe input validation using Zod

## Setup

1. Make sure you have Node.js installed
2. Install dependencies:

```bash
npm install
# or
yarn
```

## Configuration

The tool is configured in `.cursor/mcp.json` and can be accessed through Cursor's MCP server settings.

## Usage

The calculator accepts two numeric arguments and returns their sum.

### Valid Examples:

```
"10 + 12" = 22
"200 + 1200" = 1400
```

### Invalid Examples:

- "abc + 123" (Error: First argument must be a number)
- "null + 1200" (Error: First argument must be a number)

## Technical Details

- Uses @modelcontextprotocol/sdk for MCP implementation
- Input validation using Zod schema
- Runs as a Node.js server process
