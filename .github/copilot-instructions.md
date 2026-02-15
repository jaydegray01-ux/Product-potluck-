# GitHub Copilot Instructions for Product-potluck-

## Repository Overview

This is the Product-potluck- repository. This file provides instructions for GitHub Copilot coding agent to work effectively with this repository.

## Core Principles

- Make minimal, focused changes that directly address the issue
- Maintain backward compatibility unless explicitly instructed otherwise
- Follow existing code patterns and conventions in the repository
- Always validate changes through testing before finalizing

## Development Workflow

### Before Making Changes

1. **Understand the codebase**: Explore relevant files and understand the existing architecture
2. **Review the issue**: Ensure you fully understand the requirements and acceptance criteria
3. **Check for existing patterns**: Look for similar implementations in the codebase
4. **Plan your changes**: Create a checklist of changes using `report_progress` before starting

### Making Changes

1. **Make incremental changes**: Implement one logical change at a time
2. **Test frequently**: Run tests after each significant change
3. **Commit often**: Use `report_progress` to commit and push changes regularly
4. **Update documentation**: Keep documentation in sync with code changes

### Testing and Validation

1. **Run existing tests**: Ensure all existing tests pass before and after changes
2. **Add new tests**: Create tests for new functionality following existing test patterns
3. **Manual verification**: For UI changes, take screenshots to document the impact
4. **Security scanning**: Always run security checks before finalizing

## Code Style and Standards

- Follow the existing code style in the repository
- Use clear, descriptive variable and function names
- Add comments only when necessary to explain complex logic
- Keep functions small and focused on a single responsibility

## File Organization

### Do Not Modify

- `.github/agents/` - Contains instructions for other agents
- Configuration files unless specifically required
- Dependencies or build artifacts

### Key Directories

- `README.md` - Project documentation
- `.github/` - GitHub-specific configuration and workflows

## Technology Stack

This section will be updated as the project grows. Currently, this is a minimal repository.

### Future Considerations

When adding technology to this repository, consider:
- Adding appropriate build tools and configurations
- Setting up linting and formatting tools
- Implementing a testing framework
- Adding CI/CD pipelines

## Testing Guidelines

### Running Tests

- Check for test scripts in `package.json`, `Makefile`, or similar configuration files
- Run tests before committing changes
- Fix any failing tests that are related to your changes

### Writing Tests

- Follow existing test patterns in the repository
- Test edge cases and error conditions
- Ensure tests are deterministic and don't rely on external state

## Security Guidelines

### Must Do

- Never commit secrets, API keys, or sensitive credentials
- Run security scanning tools before finalizing changes
- Fix any security vulnerabilities discovered in your changes
- Use parameterized queries to prevent injection attacks

### Must Not Do

- Do not expose sensitive information in logs or error messages
- Do not introduce dependencies with known vulnerabilities
- Do not bypass authentication or authorization checks

## Pull Request Process

1. **Create a clear PR title**: Summarize the change in one line
2. **Write a detailed PR description**: Include:
   - What changed and why
   - How to test the changes
   - Any breaking changes or migrations needed
3. **Use report_progress regularly**: Keep the PR updated with your progress
4. **Request code review**: Use the `code_review` tool before finalizing
5. **Run security scans**: Use the `codeql_checker` tool to find vulnerabilities
6. **Address feedback**: Respond to review comments and update the code

## Common Commands

As the repository grows, add commonly used commands here:

```bash
# Example commands (update as project evolves)
# npm install        - Install dependencies
# npm test          - Run tests
# npm run build     - Build the project
# npm run lint      - Run linting
```

## Git Best Practices

- Write clear, descriptive commit messages
- Keep commits focused on a single logical change
- Use `git --no-pager` for git commands to avoid pager issues
- Review changes with `git --no-pager diff` before committing

## Troubleshooting

### Common Issues

- **Build failures**: Check that all dependencies are installed
- **Test failures**: Ensure tests are run from the correct directory
- **Merge conflicts**: Ask the user for help resolving merge conflicts

### Getting Help

If you encounter issues you cannot resolve:
1. Document what you've tried
2. Explain the problem clearly
3. Ask the user for guidance

## Additional Resources

- [GitHub Copilot Best Practices](https://docs.github.com/en/copilot)
- [Repository README](../README.md)

---

Last updated: 2026-02-15
