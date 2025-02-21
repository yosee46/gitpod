# Technical Context

## Core Stack
- Python 3.10+
- BeautifulSoup4
- requests
- pandas (future)

## Development Environment
- VSCode in Gitpod
- Docker-based container
- Pre-configured Python environment

## Dependency Management
```json
// .devcontainer/devcontainer.json excerpt
{
    "customizations": {
        "vscode": {
            "extensions": [
                "ms-python.python",
                "ms-python.vscode-pylance"
            ]
        }
    }
}
```

## Key Constraints
- Limited to synchronous requests
- No current proxy support
- Basic error handling implementation
