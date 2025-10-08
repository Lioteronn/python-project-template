# Big Data Learning Zone

A modern Python project template featuring best practices and essential development tools for building robust applications.

## 🚀 Features

This project includes a combination of various modern tools:

- **🔧 [uv](https://docs.astral.sh/uv/)** - Ultra-fast Python package manager and project management
- **🧹 [Ruff](https://docs.astral.sh/ruff/)** - Extremely fast Python linter and formatter (replaces Black, isort, flake8)
- **🔍 [BasedPyright](https://docs.basedpyright.com/)** - Fast static type checker (fork of Pylance)
- **🧪 [pytest](https://docs.pytest.org/)** - Testing framework with pytest-sugar for better output
- **📝 [Codespell](https://github.com/codespell-project/codespell)** - Spell checker for code
- **✨ [Rich](https://rich.readthedocs.io/)** - Beautiful terminal output and logging

## 🛠️ Development Setup

### Prerequisites

- Python 3.11+ 
- [uv](https://docs.astral.sh/uv/getting-started/installation/) package manager

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Lioteronn/python-project-template.git
cd python-project-template
```

2. Install dependencies:
```bash
uv sync --dev
```

3. Activate the virtual environment:
```bash
# Windows
.venv\Scripts\activate

# macOS/Linux
source .venv/bin/activate
```

## 🎯 Usage

### Running the Application

```bash
uv run python src/main.py
```

### Development Commands

```bash
# Run tests
uv run pytest

# Lint code
uv run ruff check .

# Format code
uv run ruff format .

# Type checking
uv run basedpyright

# Spell check
uv run codespell
```

## 📁 Project Structure

```
├── src/                    # Source code
│   └── main.py            # Main application entry point
├── tests/                 # Test files
│   └── test_example.py    # Example test file
├── .vscode/               # VS Code configuration
│   └── settings.json      # Editor settings for consistent development
├── pyproject.toml         # Project configuration and dependencies
├── uv.lock               # Dependency lock file
└── README.md             # This file
```

## ⚙️ Configuration

### VS Code Integration

The project includes VS Code settings for:
- **Automatic formatting** on save with Ruff
- **Linting** with Ruff integration
- **Type checking** with BasedPyright
- **Import organization** on save

### Tool Configuration

All tools are configured in `pyproject.toml`:
- **Ruff**: Linting rules, formatting options
- **BasedPyright**: Type checking settings
- **pytest**: Test discovery and execution
- **Codespell**: Spell checking rules

## 🧪 Testing

Run the test suite:
```bash
uv run pytest
```

Run tests with coverage:
```bash
uv run pytest --cov=src
```

## 📝 Code Quality

This project enforces code quality through:
- **Type hints** (checked by BasedPyright)
- **Code formatting** (Ruff formatter)
- **Linting** (Ruff linter)
- **Spell checking** (Codespell)
- **Testing** (pytest)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Run the quality checks:
   ```bash
   uv run ruff check .
   uv run ruff format .
   uv run basedpyright
   uv run pytest
   ```
5. Commit your changes (`git commit -m 'Add amazing feature'`)
6. Push to the branch (`git push origin feature/amazing-feature`)
7. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

*Built with ❤️ using modern Python tooling*