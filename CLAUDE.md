# Claude Code Helper Guide

## Build/Run Commands
- Run server: `uv run uvicorn server:app --host 0.0.0.0 --port 8082`
- Run all tests: `python tests.py`
- Run specific test: `python tests.py --simple` or `python tests.py --no-streaming`
- Run streaming tests only: `python tests.py --streaming-only`
- Run tool tests only: `python tests.py --tools-only`

## Code Style Guidelines
- **Imports**: Standard library first, then third-party, then local modules
- **Formatting**: 4-space indentation, 100 character line limit
- **Error Handling**: Use try/except blocks with specific error types
- **Logging**: Use the logging module with appropriate levels
- **Type Hints**: Use Python type hints for function parameters and return values
- **Documentation**: Include docstrings for functions and classes
- **Naming**: snake_case for variables/functions, PascalCase for classes
- **Tools**: Use UV for dependency management (`uv run` instead of `python`)

## Environment Variables
- `OPENAI_API_KEY`: Required for connecting to OpenAI
- `BIG_MODEL`: Controls which model is used for Sonnet (default: gpt-4o)
- `SMALL_MODEL`: Controls which model is used for Haiku (default: gpt-4o-mini)