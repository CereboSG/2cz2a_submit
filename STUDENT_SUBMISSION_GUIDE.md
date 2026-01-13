# Student Submission Guide

This guide provides detailed step-by-step instructions for students to submit their work to this repository using the automated approval system.

---

## 📋 Prerequisites

Before you begin, make sure you have:
- A GitHub account ([Sign up here](https://github.com/signup) if you don't have one)
- Git installed on your computer (optional but recommended)
- Your assignment files ready to submit

---

## 🚀 Submission Methods

You can submit your work using one of these methods:

### **Method 1: Using GitHub Web Interface** (Easiest - No Git Required)
### **Method 2: Using Git Desktop** (Recommended for Windows/Mac users)
### **Method 3: Using Git Command Line** (For advanced users)

---

## Method 1: GitHub Web Interface (Recommended for Beginners)

### Step 1: Fork the Repository

1. Go to the repository: `https://github.com/CereboSG/2cz2a_submit`
2. Click the **"Fork"** button in the top-right corner
3. Select your account as the destination
4. Wait for GitHub to create your fork (your own copy of the repository)

### Step 2: Navigate to the Appropriate Folder

1. In your forked repository, browse to the folder where you want to submit your work:
   - **`Working Folder/`** - For general work and practice
   - **`Exercises/`** - For exercise submissions
   - **`Notes/`** - For notes and study materials

2. If you need to create a new folder:
   - Click **"Add file"** → **"Create new file"**
   - Type the folder name followed by `/` (e.g., `Exercises/Assignment_1/`)
   - Then type a filename (you can delete this placeholder file later)

### Step 3: Upload Your Files

1. Click the **"Add file"** button
2. Select **"Upload files"**
3. **Drag and drop** your files into the upload area, or click **"choose your files"** to browse
4. Supported file types:
   - Python files (`.py`)
   - Jupyter notebooks (`.ipynb`)
   - Documents (`.txt`, `.pdf`, `.md`, `.doc`, `.docx`)
   - Data files (`.csv`, `.json`, `.xlsx`)
   - Images (`.png`, `.jpg`, `.gif`, `.svg`)
   - And more (see [AUTO_APPROVAL.md](AUTO_APPROVAL.md) for full list)

5. Files must be **under 10MB** each

### Step 4: Commit Your Changes

1. Scroll down to the **"Commit changes"** section
2. Write a descriptive commit message, for example:
   - `Add Assignment 1 submission`
   - `Upload Exercise 7 Python files`
   - `Submit Week 3 homework`

3. Select **"Commit directly to the main branch"**
4. Click **"Commit changes"**

### Step 5: Create a Pull Request

1. Go back to the main page of your forked repository
2. You should see a banner saying **"This branch is X commits ahead of CereboSG:main"**
3. Click **"Contribute"** → **"Open pull request"**
4. Fill in the pull request details:
   - **Title**: Brief description (e.g., "Submit Assignment 1 - John Doe")
   - **Description**: Optional details about your submission
5. Click **"Create pull request"**

### Step 6: Wait for Automatic Approval

1. The automated system will check your files (usually takes 30-60 seconds)
2. You'll see a green checkmark ✅ if all files are valid
3. The PR will be automatically approved and merged
4. You'll receive a notification when your submission is accepted

**What happens if something is wrong?**
- You'll see a comment explaining what needs to be fixed
- Common issues:
  - File type not allowed (e.g., `.exe`, `.sh`)
  - File too large (over 10MB)
  - Trying to modify protected files

---

## Method 2: Using GitHub Desktop

### Step 1: Install GitHub Desktop

1. Download from: https://desktop.github.com/
2. Install and sign in with your GitHub account

### Step 2: Fork and Clone

1. Go to `https://github.com/CereboSG/2cz2a_submit` in your browser
2. Click **"Fork"** to create your copy
3. In GitHub Desktop, go to **File** → **Clone Repository**
4. Select your fork from the list
5. Choose where to save it on your computer
6. Click **"Clone"**

### Step 3: Add Your Files

1. Open the cloned folder on your computer (File Explorer/Finder)
2. Navigate to the appropriate subfolder:
   - `Working Folder/`
   - `Exercises/`
   - `Notes/`
3. Copy your assignment files into the folder
4. You can organize files in subfolders (e.g., `Exercises/Week1/`, `Exercises/Assignment1/`)

### Step 4: Commit and Push

1. Return to GitHub Desktop
2. You'll see your added files listed on the left
3. In the bottom-left corner:
   - **Summary**: Write a brief commit message (e.g., "Add Assignment 1")
   - **Description** (optional): Add more details
4. Click **"Commit to main"**
5. Click **"Push origin"** to upload your changes to GitHub

### Step 5: Create Pull Request

1. In GitHub Desktop, click **"Preview Pull Request"**
2. Review the changes
3. Click **"Create pull request"**
4. Your browser will open with the PR form
5. Add a title and description
6. Click **"Create pull request"**
7. Wait for automatic approval (30-60 seconds)

---

## Method 3: Using Git Command Line

### Step 1: Fork and Clone

```bash
# Fork the repository first on GitHub.com, then:

# Clone your fork
git clone https://github.com/YOUR_USERNAME/2cz2a_submit.git
cd 2cz2a_submit

# Add upstream remote (original repository)
git remote add upstream https://github.com/CereboSG/2cz2a_submit.git
```

### Step 2: Create a Branch (Optional but Recommended)

```bash
# Create and switch to a new branch
git checkout -b submission/your-name-assignment1

# Or work directly on main if you prefer
```

### Step 3: Add Your Files

```bash
# Copy your files to the appropriate folder, then:

# Add all new files
git add .

# Or add specific files
git add "Working Folder/homework.py"
git add "Exercises/Assignment1/"

# Check what will be committed
git status
```

### Step 4: Commit Your Changes

```bash
# Commit with a descriptive message
git commit -m "Add Assignment 1 submission - John Doe"

# If you want a more detailed message
git commit -m "Add Assignment 1 submission" -m "Includes: task1.py, task2.py, report.pdf"
```

### Step 5: Push to Your Fork

```bash
# Push to your fork on GitHub
git push origin main

# Or if you created a branch:
git push origin submission/your-name-assignment1
```

### Step 6: Create Pull Request

```bash
# Option 1: Use GitHub CLI (if installed)
gh pr create --title "Submit Assignment 1 - John Doe" --body "Assignment 1 submission"

# Option 2: Use the web interface
# Go to your fork on GitHub.com
# Click "Contribute" → "Open pull request"
# Fill in the details and submit
```

---

## ✅ Verification Checklist

Before submitting, verify:

- [ ] All files are in the correct folder
- [ ] File names are clear and descriptive
- [ ] Each file is under 10MB
- [ ] File types are allowed (see list below)
- [ ] You're not modifying protected files (`.github/`, `LICENSE`, `README.md`)
- [ ] Your commit message is descriptive

### ✅ Allowed File Types

- Python: `.py`
- Jupyter Notebooks: `.ipynb`
- Documents: `.txt`, `.md`, `.pdf`, `.doc`, `.docx`, `.ppt`, `.pptx`
- Data: `.csv`, `.json`, `.xlsx`, `.xls`
- Databases: `.db`, `.sqlite`, `.sqlite3`
- Web: `.html`, `.css`, `.js`
- SQL: `.sql`
- Images: `.png`, `.jpg`, `.jpeg`, `.gif`, `.svg`
- Archives: `.zip`

### ⚠️ File Types NOT Allowed (Will Require Manual Review)

- Executables: `.exe`, `.app`, `.dmg`
- Scripts: `.sh`, `.bat`, `.cmd`
- Configuration: `.yml`, `.yaml` (in `.github/` folder)
- System: `.dll`, `.so`

---

## 🆘 Troubleshooting

### "My PR wasn't auto-approved"

Check the workflow run for details:
1. Go to your pull request
2. Click on the "Checks" tab
3. Look for the "Auto-Approve File Uploads" workflow
4. Click on it to see what went wrong

Common issues:
- **File too large**: Split into smaller files or compress
- **Wrong file type**: Convert to an allowed format
- **Protected path**: Don't modify `.github/`, `LICENSE`, or main `README.md`

### "I made a mistake in my submission"

If your PR is still open:
1. Add more commits to the same branch
2. The PR will automatically update

If your PR was already merged:
1. Create a new PR with corrections
2. Name it clearly (e.g., "Fix Assignment 1 - Corrected task2.py")

### "I can't find my files after merging"

After your PR is merged:
1. Go to the main repository: `https://github.com/CereboSG/2cz2a_submit`
2. Navigate to the folder where you submitted
3. Your files should be there
4. You can view them directly on GitHub

### "The automatic check is taking too long"

- Usually completes in 30-60 seconds
- If it takes more than 5 minutes, there might be an issue
- Check the Actions tab for workflow status
- Contact the repository administrator if needed

---

## 📞 Getting Help

If you encounter issues:

1. **Check the documentation**: [AUTO_APPROVAL.md](AUTO_APPROVAL.md)
2. **Review your PR comments**: The bot explains what went wrong
3. **Ask your instructor**: They can help with specific assignment requirements
4. **Check GitHub's documentation**: https://docs.github.com/

---

## 🎯 Quick Reference

### First-Time Setup
1. Fork repository
2. Clone to your computer (optional)

### Each Submission
1. Add files to appropriate folder
2. Commit with descriptive message
3. Push to your fork
4. Create pull request
5. Wait for auto-approval (~1 minute)

### After Submission
- Your work is automatically merged
- Files appear in the main repository
- You can submit corrections anytime

---

## 🎓 Best Practices

1. **Organize your files**: Use subfolders for different assignments
   ```
   Exercises/
   ├── Assignment1/
   │   ├── task1.py
   │   └── task2.py
   └── Assignment2/
       └── solution.ipynb
   ```

2. **Use clear file names**: 
   - ✅ Good: `assignment1_task1.py`, `week3_exercise.ipynb`
   - ❌ Bad: `stuff.py`, `final_final_v2.py`

3. **Write good commit messages**:
   - ✅ Good: "Add Week 3 homework submission"
   - ❌ Bad: "update", "changes", "asdf"

4. **Submit early**: Don't wait until the last minute in case there are issues

5. **One PR per assignment**: Don't mix multiple assignments in one PR

6. **Keep files small**: If needed, split large files or compress them

---

## 📝 Example Workflow

Here's what a typical submission looks like:

```
1. John forks the repository to his account
2. John clones his fork to his computer
3. John creates a folder: Exercises/Week1/
4. John adds his files: task1.py, task2.py, data.csv
5. John commits: "Add Week 1 exercise submission"
6. John pushes to his fork
7. John creates a pull request: "Week 1 Submission - John Doe"
8. The automated system checks:
   ✓ task1.py - Valid Python file
   ✓ task2.py - Valid Python file
   ✓ data.csv - Valid CSV file
   ✓ All files under 10MB
   ✓ No protected paths modified
9. PR is auto-approved and merged in ~45 seconds
10. John's files now appear in the main repository
11. Submission complete! ✅
```

---

*Last updated: January 2026*
