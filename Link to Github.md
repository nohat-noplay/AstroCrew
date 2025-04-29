## How to Link a Local Folder to GitHub

## 1. Create a New GitHub Repository
- Go to [github.com](https://github.com/).
- Click **New Repository**.
- Name your repo (e.g., `airline-management-system`).
- **Important:**
    - Leave **README**, **.gitignore**, and **License** **unchecked**.
- Click **Create Repository**.
---
## 2. Open Terminal Inside Your Project Folder
- Navigate to your folder on your computer.
- Open **Terminal** / **Git Bash** inside the folder.
---
## 3. Initialise Git
`git init`

---
## 4. Add and Commit Your Files

`git add . git commit -m "Initial commit: upload project files"`

---
## 5. Connect to GitHub

`git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git`

---
## 6. Push to GitHub

`git branch -M main`
`git push -u origin main`

---
#  Notes

- If you get a "fetch first" error, run:
    `git pull origin main --allow-unrelated-histories`
    then push again.
    
- After this setup, to update your project:
    `git add . git commit -m "Your commit message" git push`
    