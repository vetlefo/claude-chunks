# Claude Chunks

An intelligent document chunking MCP server optimized for Claude context windows. Split large documents into meaningful, context-aware chunks that can be progressively processed by Claude.

## Overview

Claude Chunks helps you process large documents (like books, theses, or long papers) by:
1. Breaking them into meaningful sections
2. Generating rich summaries of each section
3. Maintaining context and connections between sections
4. Formatting output for optimal Claude context reuse

## Installation

```bash
# Clone the repository
git clone https://github.com/vetlefo/claude-chunks.git
cd claude-chunks

# Install dependencies
npm install

# Build the project
npm run build
```

## Usage with Claude Desktop

1. Add to Claude Desktop config:
```json
{
  "mcpServers": {
    "claude-chunks": {
      "command": "node",
      "args": ["/path/to/claude-chunks/dist/index.js"]
    }
  }
}
```

2. Restart Claude Desktop
3. Use the `chunk_document` tool in your conversations

## Development Roadmap

### Phase 1: Core Functionality
- [ ] Basic MCP server setup
- [ ] Smart document chunking
- [ ] Section summarization
- [ ] Context preservation

### Phase 2: Enhancements
- [ ] Multiple document formats
- [ ] Custom chunking strategies
- [ ] Enhanced metadata tracking
- [ ] Claude-optimized formatting

### Phase 3: Advanced Features
- [ ] Cross-reference tracking
- [ ] Technical term extraction
- [ ] Theme detection
- [ ] Progressive loading

## Contributing

Contributions are welcome! Please see our [Contributing Guide](CONTRIBUTING.md) for details.

## License

MIT