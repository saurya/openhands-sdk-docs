# OpenHands Software Agent SDK - Mintlify Documentation

This repository contains Mintlify-based technical documentation for the [OpenHands Software Agent SDK](https://github.com/OpenHands/software-agent-sdk).

## Documentation Structure

### Configuration
- **`mint.json`**: Mintlify configuration file defining navigation, branding, and settings

### Documentation Pages
- **`docs/introduction.mdx`**: Overview, features, and quick start guide
- **`docs/setup.mdx`**: Installation and environment configuration
- **`docs/architecture.mdx`**: Core concepts, component architecture, and design patterns
- **`docs/usage.mdx`**: Practical examples and common usage patterns
- **`docs/api.mdx`**: Complete API reference for all public interfaces

## Documentation Coverage

### Introduction (`docs/introduction.mdx`)
- Project overview and purpose
- Key features and capabilities
- Quick example code
- Repository structure
- Community resources

### Setup (`docs/setup.mdx`)
- Installation methods (UV, pip, development setup)
- Environment configuration (LLM API keys, Agent Server)
- Verification steps
- Development commands (testing, linting, building)
- Agent Server setup
- Troubleshooting guide

### Architecture (`docs/architecture.mdx`)
- Core components:
  - Agent (`openhands-sdk/openhands/sdk/agent/`)
  - LLM (`openhands-sdk/openhands/sdk/llm/`)
  - Conversation (`openhands-sdk/openhands/sdk/conversation/`)
  - Tool (`openhands-sdk/openhands/sdk/tool/`, `openhands-tools/openhands/tools/`)
  - Workspace (`openhands-sdk/openhands/sdk/workspace/`, `openhands-workspace/`)
- Package architecture (monorepo structure)
- Data flow and execution lifecycle
- Event system
- Advanced features (Skills, Plugins, Sub-agents, MCP)
- Agent Server architecture
- Security and isolation
- Extension points

### Usage (`docs/usage.mdx`)
- Basic usage patterns (hello world, async)
- Working with tools (built-in, custom, configuration)
- LLM configuration (multiple providers, streaming, fallback)
- Conversation management (persistence, callbacks, confirmation)
- Workspaces (local, remote, Docker)
- Advanced features (skills, sub-agents, MCP, browser automation)
- Agent Server usage (REST, WebSocket)
- Common patterns (planning, iteration, multi-agent)
- Testing strategies
- 40+ example references

### API Reference (`docs/api.mdx`)
- Core classes (Agent, LLM, Conversation, Tool, Workspace)
- Message types
- Event system
- Plugin system
- Skills and sub-agents
- Context management
- MCP integration
- Observability
- Error handling
- Utility functions
- Agent Server API (REST endpoints, WebSocket)
- Type definitions
- Best practices
- Package exports

## Source Repository Information

**Source**: https://github.com/OpenHands/software-agent-sdk

The documentation is based on version **1.13.1** of the SDK and covers:
- **openhands-sdk**: Core SDK functionality
- **openhands-tools**: Built-in tools for agents
- **openhands-workspace**: Workspace implementations (local, Docker, etc.)
- **openhands-agent-server**: REST/WebSocket API server

### Key Source File References

Documentation references specific files from the source repository:

**Core SDK** (`openhands-sdk/openhands/sdk/`)
- `agent/agent.py` - Agent implementation
- `llm/llm.py` - LLM communication
- `conversation/conversation.py` - Conversation management
- `tool/tool.py` - Tool framework
- `workspace/workspace.py` - Workspace abstractions

**Built-in Tools** (`openhands-tools/openhands/tools/`)
- `terminal/` - Shell execution
- `file_editor/` - File operations
- `task_tracker/` - Task management
- `browser_use/` - Browser automation
- `delegate/` - Agent delegation

**Agent Server** (`openhands-agent-server/openhands/agent_server/`)
- `api.py` - FastAPI application
- `conversation_router.py` - Conversation endpoints
- `sockets.py` - WebSocket handling
- `README.md` - Server documentation

**Examples** (`examples/`)
- `01_standalone_sdk/` - 44 SDK usage examples
- `02_remote_agent_server/` - Remote workspace examples
- `03_github_workflows/` - CI/CD integration

## Viewing the Documentation

To view this documentation with Mintlify:

1. Install Mintlify CLI:
```bash
npm i -g mintlify
```

2. Run the development server:
```bash
cd /path/to/target
mintlify dev
```

3. Open your browser to `http://localhost:3000`

## Notes

- Logo and favicon paths in `mint.json` reference assets that should be added to the repository
- All code examples are based on actual implementation patterns from the source repository
- File paths and module references are accurate to the source repository structure
- API documentation covers the public API as exported from `openhands.sdk.__init__.py`
- Built-in tools are documented from `openhands-tools/openhands/tools/`
- Examples reference actual files in the `examples/` directory

## Maintenance

When updating this documentation:

1. Verify file paths match the current source repository structure
2. Check that version numbers are current
3. Ensure code examples reflect current API
4. Update examples references if new examples are added
5. Review Agent Server API documentation against actual endpoints

## Additional Resources

- **Official Documentation**: https://docs.openhands.dev/sdk
- **GitHub Repository**: https://github.com/OpenHands/software-agent-sdk
- **Slack Community**: https://openhands.dev/joinslack
- **Tech Report**: https://arxiv.org/abs/2511.03690
