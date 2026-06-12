# Setup and Usage Instructions

## Table of Contents

1. [Prerequisites](#prerequisites)
2. [System Requirements](#system-requirements)
3. [Initial Setup](#initial-setup)
4. [Install Dependencies](#install-dependencies)
5. [Setup and Usage Instructions](#setup-and-usage-instructions)
6. [Available Commands](#available-commands)
7. [Development Commands](#development-commands)
8. [Running Scripts](#running-scripts)
9. [Best Practices](#best-practices)
10. [Troubleshooting](#troubleshooting)
11. [Extending the Application](#extending-the-application)
12. [External Resources](#external-resources)
13. [Version](#version)
14. [Last Updated](#last-updated)

## Prerequisites

### System Requirements

- **Node.js**: Version 12 or higher
- **npm**: Package manager
- **Gmail Account**: Dummy account recommended for testing
- **Google Cloud Project**: With Gmail API enabled
- **Internet Connection**: For Gmail API access

### Gmail Account Requirements

- Active Gmail account
- Google Cloud Project with Gmail API enabled
- OAuth2 credentials

## Initial Setup

1. Open the project in your IDE (VSCode recommended)

### Install Dependencies

Install dependencies:

```bash
npm install
```

### Setup and Usage Instructions

### 1. Gmail API Credentials Setup

1. Create a Google Cloud Project
2. Enable the Gmail API
3. Create OAuth2 credentials
4. Download credentials JSON file
5. Place credentials in the project

### 2. Configure Application

1. Configure source directory path
2. Define file extensions to scan
3. Set output directory for reports and logs

## Available Commands

### Development Commands

**Start the application:**

```bash
npm start
```

**Backup project:**

```bash
npm run backup
```

### Running Scripts

\*\*Run the grammar/spelling checker:

```bash
npm start
```

## Best Practices

### Before Running

1. Use a dummy Gmail account for testing
2. Review configuration before running
3. Backup files to process
4. Start with a small set of files

### Development

1. Keep code clean and readable
2. Always handle errors with unique codes
3. Log all important operations
4. Keep documentation up to date

## Troubleshooting

### Common Issues

1. Authentication errors
   - Verify Gmail API credentials
   - Check OAuth2 setup
2. File access issues
   - Check file permissions
   - Verify file paths exist
3. API rate limits
   - Check Google API quotas
   - Implement rate limiting

## Extending the Application

To extend the application:

1. Add new file types
2. Add new reporting formats
3. Integrate with other APIs
4. Add new analysis features

## External Resources

- [Gmail API Documentation](https://developers.google.com/gmail/api)
- [OAuth 2.0 for Desktop Apps](https://developers.google.com/identity/protocols/oauth2/native-app)
- [Node.js Documentation](https://nodejs.org/docs/)

## Version

1.0.0

## Last Updated

June 2026

## Setup Instructions

1. Open the project in your IDE (VSCode recommended)
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the application:
   ```bash
   npm start
   ```

## Configuration

Before running the application, you'll need to:

1. **Set up Gmail API credentials**:
   - Create a Google Cloud Project
   - Enable the Gmail API
   - Download OAuth2 credentials
   - Place credentials in the appropriate configuration file

2. **Configure file paths**:
   - Set the source directory path for files to be checked
   - Configure output directory for results/logs

3. **Set up scanning parameters**:
   - Define file extensions to scan
   - Configure grammar/spelling check settings

## Running the Application

### Main Script

Run the grammar/spelling checker:

```bash
npm start
```

**What it does:**

1. Authenticates with Gmail API
2. Scans files from the configured directory
3. Creates email drafts with file contents
4. Checks grammar and spelling mistakes
5. Logs recommended fixes
6. Generates a report of findings

## Project Structure

### Documentation Files (`misc/documents/`)

- `todo_tasks.txt` - Planned features and tasks
- `complete_tasks.txt` - Completed development tasks
- `finalize_tasks.txt` - Pre-release checklist
- `error_index.txt` - Error code reference

### Backup Files (`misc/backups/`)

Backup directory for code snapshots before changes.

## Development Workflow

### Before Making Changes

1. Create a backup:

   ```bash
   npm run backup
   ```

   or manually backup to `misc/backups/`

2. Review the maintenance checklist in `misc/documents/todo_tasks.txt`

### After Making Changes

1. Test that everything works correctly
2. Update documentation if needed
3. Commit and push to Git repository
4. Update iOmega backup (every couple of days)

## Error Codes

All errors include a unique serial number (starting from 1000000) for easy identification. See `misc/documents/error_index.txt` for the complete error code reference.

## Development Guidelines

The project follows these principles:

- Clean, simple, readable code
- Clear and consistent naming conventions
- Modular code structure
- Short sentences in comments
- No comments inside function bodies
- Comprehensive error handling with unique error codes

## Gmail API Integration

### Authentication

The application uses OAuth2 for Gmail authentication. Follow these steps:

1. Set up credentials in Google Cloud Console
2. Download client configuration
3. Run the authentication flow on first use
4. Access tokens are managed automatically

### Email Operations

- Creates draft emails with file contents
- Runs grammar/spelling checks via Gmail's interface
- Extracts and logs suggested corrections

## Notes

- Requires a Gmail account (dummy account recommended for testing)
- Internet connection required for Gmail API access
- All file scans are logged for review
- Results include both detected issues and recommended fixes

## Planned Features

See `misc/documents/todo_tasks.txt` for the complete list of planned features and improvements.

## Author

- **Or Assayag** - _Initial work_ - [orassayag](https://github.com/orassayag)
- Or Assayag <orassayag@gmail.com>
- GitHub: https://github.com/orassayag
- StackOverflow: https://stackoverflow.com/users/4442606/or-assayag?tab=profile
- LinkedIn: https://linkedin.com/in/orassayag
