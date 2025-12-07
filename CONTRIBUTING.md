# Contributing to TPU Inference Server

Thank you for your interest in contributing to TPU Inference Server! This document provides guidelines and instructions for contributing.

## How to Contribute

### Reporting Bugs

- Check existing issues to avoid duplicates
- Use a clear, descriptive title
- Include steps to reproduce the issue
- Specify your environment (Python version, TPU type, OS)
- Include relevant logs or error messages

### Suggesting Features

- Open an issue describing the feature
- Explain the use case and why it would be useful
- Be open to discussion about implementation approaches

### Submitting Pull Requests

1. Fork the repository
2. Create a feature branch from `main`:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Make your changes
4. Run tests and linting:
   ```bash
   pip install -e ".[dev]"
   pytest
   black src/
   ruff check src/ --fix
   ```
5. Commit your changes with a descriptive message
6. Push to your fork and open a pull request

## Development Setup

```bash
# Clone your fork
git clone https://github.com/YOUR_USERNAME/tpu-inference-server.git
cd tpu-inference-server

# Install in development mode
pip install -e ".[dev]"

# Run tests
pytest

# Format code
black src/

# Lint code
ruff check src/ --fix
```

## Code Style

- Follow PEP 8 guidelines
- Use [Black](https://github.com/psf/black) for formatting (line length: 100)
- Use [Ruff](https://github.com/astral-sh/ruff) for linting
- Add type hints where possible
- Write docstrings for public functions and classes

## Testing

- Add tests for new features
- Ensure all tests pass before submitting a PR
- Test on TPU hardware when possible (or document if TPU-specific testing is needed)

## Pull Request Guidelines

- Keep PRs focused on a single change
- Update documentation if needed
- Add tests for new functionality
- Ensure CI passes

## Code of Conduct

- Be respectful and inclusive
- Provide constructive feedback
- Focus on the code, not the person

## Questions?

Open an issue for any questions about contributing.

## License

By contributing, you agree that your contributions will be licensed under the MIT License.
