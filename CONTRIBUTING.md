# Contributing

Contributions to this project are [released](https://help.github.com/articles/github-terms-of-service/#6-contributions-under-repository-license) to the public under the [project's open source license](LICENSE).

Everyone is welcome to contribute to this project. Contributing doesn't just mean submitting pull requests—there are many different ways for you to get involved, including answering questions, reporting issues, improving documentation, or suggesting new features.

## How to Contribute

### Reporting Issues

If you find a bug or have a feature request:
1. Check if the issue already exists in the [GitHub Issues](https://github.com/orassayag/gmail-detector/issues)
2. If not, create a new issue with:
   - Clear title and description
   - Steps to reproduce (for bugs)
   - Expected vs actual behavior
   - Error codes (if applicable)
   - Your environment details (OS, Node version)

### Submitting Pull Requests

1. Fork the repository
2. Create a new branch for your feature/fix:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Make your changes following the code style guidelines below
4. Test your changes thoroughly
5. Commit with clear, descriptive messages
6. Push to your fork and submit a pull request

### Code Style Guidelines

This project uses:
- **Node.js** for runtime
- **npm** for package management

Before submitting:
```bash
# Install dependencies
npm install

# Test the application
npm start
```

### Coding Standards

1. **Functions with 3+ parameters**: Use object parameters with proper types
2. **Error handling**: All errors must include unique error codes (see `misc/documents/error_index.txt`)
3. **Comments**: Use clear and easy-to-understand language. Write in short sentences.
4. **Code style**: Follow the patterns in the existing codebase
5. **No comments inside functions**: Keep function bodies clean
6. **Naming**: Use clear, descriptive names for variables and functions

### Adding New Features

When adding new features:
1. Update the todo tasks in `misc/documents/todo_tasks.txt`
2. Add error codes and update `misc/documents/error_index.txt`
3. Update documentation files
4. Test thoroughly
5. Update the README.md with any new functionality

### Error Code Management

When adding new errors:
1. Use the next available error code from `misc/documents/error_index.txt`
2. Format: `[ERROR-XXXXXXX]` at the start of the error message
3. Document the error in `misc/documents/error_index.txt`
4. Update the "Last error number" line

## Questions or Need Help?

Please feel free to contact me with any question, comment, pull-request, issue, or any other thing you have in mind.

* Or Assayag <orassayag@gmail.com>
* GitHub: https://github.com/orassayag
* StackOverflow: https://stackoverflow.com/users/4442606/or-assayag?tab=profile
* LinkedIn: https://linkedin.com/in/orassayag

Thank you for contributing! 🙏
