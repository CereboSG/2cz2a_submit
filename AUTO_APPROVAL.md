# Automated File Upload System

This repository is configured as an automated file upload platform. Pull requests containing approved file types will be automatically reviewed and merged.

## How It Works

When you create a pull request:

1. The GitHub Actions workflow automatically checks all files in your PR
2. Files are checked against:
   - **Allowed file patterns** (e.g., .py, .ipynb, .txt, .pdf)
   - **File size limits** (maximum 10MB per file)
   - **Protected paths** (e.g., .github/, LICENSE, README.md)
3. If all files pass these checks, the PR is automatically approved and merged
4. If any checks fail, the PR will require manual review

## Allowed File Types

The following file types are automatically approved:

- **Programming Files**: `.py`, `.js`, `.html`, `.css`, `.sql`
- **Documents**: `.txt`, `.md`, `.pdf`, `.doc`, `.docx`, `.ppt`, `.pptx`
- **Data Files**: `.json`, `.csv`, `.xlsx`, `.xls`, `.db`, `.sqlite`, `.sqlite3`
- **Notebooks**: `.ipynb` (Jupyter notebooks)
- **Images**: `.png`, `.jpg`, `.jpeg`, `.gif`, `.svg`
- **Archives**: `.zip`

## Submitting Files

To submit files to this repository:

1. Fork this repository (if you don't have write access)
2. Add your files to the appropriate folder (Notes, Exercises, Working Folder, etc.)
3. Create a pull request
4. The system will automatically approve and merge your PR if all files are valid types

## Notes

- Only files with allowed extensions will be auto-approved
- Files must not exceed 10MB in size
- Protected paths (.github/, LICENSE, README.md) cannot be modified via auto-approval
- Files without extensions or with unusual extensions will require manual review
- This automation helps streamline the submission process for students and contributors
- The workflow runs automatically on every pull request
- Merge commits preserve the full history of changes (not squashed)

## Security Safeguards

To protect the repository, the automated system includes:

1. **File Type Restrictions**: Only pre-approved file extensions are allowed
2. **Size Limits**: Files cannot exceed 10MB
3. **Protected Paths**: Critical files and configuration cannot be auto-merged
4. **Transparent Logging**: All checks and results are logged in the workflow run

⚠️ **Note**: While automated, this system still relies on repository administrators to monitor for malicious content. Always review the activity log periodically.

## Disabling Auto-Approval

Repository administrators can disable auto-approval by:
1. Going to Settings → Actions → General
2. Disabling the "Auto-Approve File Uploads" workflow
3. Or by deleting the `.github/workflows/auto-approve-uploads.yml` file
