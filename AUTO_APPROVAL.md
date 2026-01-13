# Automated File Upload System

This repository is configured as an automated file upload platform. Pull requests containing approved file types will be automatically reviewed and merged.

## How It Works

When you create a pull request:

1. The GitHub Actions workflow automatically checks all files in your PR
2. If all files match the allowed file patterns, the PR is automatically approved and merged
3. If any files don't match allowed patterns, the PR will require manual review

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
- Files without extensions or with unusual extensions will require manual review
- This automation helps streamline the submission process for students and contributors
- The workflow runs automatically on every pull request

## Disabling Auto-Approval

Repository administrators can disable auto-approval by:
1. Going to Settings → Actions → General
2. Disabling the "Auto-Approve File Uploads" workflow
3. Or by deleting the `.github/workflows/auto-approve-uploads.yml` file
