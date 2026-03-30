# Instructions

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

* **Or Assayag** - *Initial work* - [orassayag](https://github.com/orassayag)
* Or Assayag <orassayag@gmail.com>
* GitHub: https://github.com/orassayag
* StackOverflow: https://stackoverflow.com/users/4442606/or-assayag?tab=profile
* LinkedIn: https://linkedin.com/in/orassayag
