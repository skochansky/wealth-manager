# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Wealth Manager - A FastAPI application managed with Poetry. Requires Python 3.13+.

## Development Commands

### Dependency Management
```bash
poetry install                    # Install dependencies
poetry add <package>              # Add dependency
poetry add --group dev <package>  # Add dev dependency
poetry update                     # Update dependencies
```

### Running the Application
```bash
poetry run uvicorn main:app --reload              # Run dev server with auto-reload
poetry run uvicorn main:app --host 0.0.0.0 --port 8000  # Run on specific host/port
```

### Testing
```bash
poetry run pytest                                 # Run all tests
poetry run pytest tests/test_file.py              # Run specific test file
poetry run pytest tests/test_file.py::test_name   # Run specific test
poetry run pytest -v                              # Verbose output
poetry run pytest --cov                           # Run with coverage
```

## Architecture

Project is in initial setup phase. No FastAPI application structure exists yet.