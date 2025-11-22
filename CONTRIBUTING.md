# Contributing Guidelines

Thank you for your interest in contributing! This document provides guidelines for contributing to this project.

## Code of Conduct

Be respectful, inclusive, and professional in all interactions.

## Getting Started

1. Fork the repository
2. Clone your fork: `git clone https://github.com/your-username/repo-name.git`
3. Create a feature branch: `git checkout -b feature/amazing-feature`
4. Make your changes
5. Run tests and linters
6. Commit and push
7. Create a Pull Request

## Development Setup

### Prerequisites
- Python 3.10+ (for Python repos) or Node.js 18+ (for JavaScript repos)
- Git
- Docker (optional, for local testing)

### Installation
```bash
# Python projects
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
pip install -r requirements-dev.txt  # development dependencies

# Node.js projects
npm install
```

## Code Style

### Python
- Follow PEP 8 style guide
- Use type hints for all functions
- Maximum line length: 88 characters (Black default)
- Enforced by: `ruff` linter

```bash
# Run linter
ruff check .

# Run formatter
ruff format .
```

### JavaScript/TypeScript
- Follow Standard JS style
- Use TypeScript for type safety
- Maximum line length: 100 characters
- Enforced by: `eslint` + `prettier`

```bash
# Run linter
npm run lint

# Run formatter
npm run format
```

## Testing Requirements

All new code must include tests with minimum 70% code coverage.

### Python
```bash
# Run tests
pytest

# Run with coverage
pytest --cov=. --cov-report=html
```

### JavaScript/TypeScript
```bash
# Run tests
npm test

# Run with coverage
npm test -- --coverage
```

## Commit Message Format

Use [Conventional Commits](https://www.conventionalcommits.org/) format:

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes (formatting, etc.)
- `refactor`: Code refactoring
- `test`: Adding or updating tests
- `chore`: Maintenance tasks

### Examples
```
feat(api): add FHIR terminology endpoint

Implements SNOMED CT and LOINC code lookups via HAPI FHIR API.
Closes #123

fix(dicom): resolve SR validation error

Fixes TID 1500 measurement group encoding issue.
```

## Pull Request Process

1. **Update documentation** if you changed APIs or added features
2. **Add tests** for new functionality
3. **Run all tests** and ensure they pass
4. **Run linters** and fix any issues
5. **Update CHANGELOG.md** with your changes
6. **Request review** from at least one maintainer
7. **Address review comments** promptly
8. **Squash commits** before merging (if requested)

### PR Checklist
- [ ] Tests added and passing
- [ ] Code follows style guidelines
- [ ] Documentation updated
- [ ] CHANGELOG.md updated
- [ ] No merge conflicts
- [ ] CI/CD pipeline passing

## Branch Naming

Use descriptive branch names:
- `feature/add-graphrag-indexing`
- `fix/orthanc-connection-timeout`
- `docs/update-api-reference`
- `refactor/simplify-sr-builder`

## Questions or Issues?

- Create an issue for bugs or feature requests
- Use discussions for questions
- Email: bryankaufman@mac.com for private matters

## License

By contributing, you agree that your contributions will be licensed under the same license as the project.

Thank you for contributing!
