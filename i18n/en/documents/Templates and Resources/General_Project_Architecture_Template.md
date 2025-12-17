# General Project Architecture Template

## 1️⃣ Standard Structure for Python Web/API Projects

```
ProjectName/
├── README.md                 # Project description document
├── LICENSE                   # Open-source license
├── requirements.txt          # Dependency management (pip)
├── pyproject.toml           # Modern Python project configuration (recommended)
├── setup.py                 # Package installation script (if used as a library)
├── .gitignore              # Git ignore file
├── .env                    # Environment variables (not committed to Git)
├── .env.example            # Example environment variables
├── CLAUDE.md              # Claude persistent context
├── AGENTS.md              # Codex persistent context
├── Sublime-Text.txt                   # For demands and notes, for myself, and CLI session recovery commands ^_^
│
├── docs/                   # Documentation directory
│   ├── api.md             # API documentation
│   ├── development.md     # Development guide
│   └── architecture.md    # Architecture description
│
├── scripts/               # Script tools
│   ├── deploy.sh          # Deployment script
│   ├── backup.sh          # Backup script
│   └── init_db.sh         # Database initialization
│
├── tests/                 # Test code
│   ├── __init__.py
│   ├── conftest.py        # Pytest configuration
│   ├── unit/              # Unit tests
│   ├── integration/       # Integration tests
│   └── test_config.py     # Configuration tests
│
├── src/                   # Source code (recommended)
│   ├── __init__.py
│   ├── main.py           # Program entry point
│   ├── app.py            # Flask/FastAPI application
│   ├── config.py         # Configuration management
│   │
│   ├── core/             # Core business logic
│   │   ├── __init__.py
│   │   ├── models/       # Data models
│   │   ├── services/     # Business services
│   │   └── utils/        # Utility functions
│   │
│   ├── api/              # API interface layer
│   │   ├── __init__.py
│   │   ├── v1/           # Version 1
│   │   └── dependencies.py
│   │
│   ├── data/             # Data processing
│   │   ├── __init__.py
│   │   ├── repository/   # Data access layer
│   │   └── migrations/   # Database migrations
│   │
│   └── external/         # External services
│       ├── __init__.py
│       ├── clients/      # API clients
│       └── integrations/ # Integration services
│
├── logs/                  # Log directory (not committed to Git)
│   ├── app.log
│   └── error.log
│
└── data/                  # Data directory (not committed to Git)
    ├── raw/               # Raw data
    ├── processed/         # Processed data
    └── cache/             # Cache
```