## Step 1: Create a Virtual Environment
If you haven't already been using a virtual environment:

`python -m venv .venv`
`.\.venv\Scripts\Activate` OR gitbash: `source .venv/Scripts/activate`

## Step 2: Install Your Project Dependencies

Install all the libraries your project needs:
`pip install <your-packages>`

## Step 3: Save Installed Packages to `requirements.txt`

Generate the requirements.txt:
`pip freeze > requirements.txt`

## Step 4: Test the Setup (Simulate a Fresh Environment)

Pretend you are a new user by setting up a **fresh** environment:
1. Create a new environment:
 `python -m venv test_env`
 2. Activate it
`.\test_env\Scripts\activate` OR gitbash: `source test_env/Scripts/activate`
3. Install all dependencies from requirements.txt
 `pip install -r requirements.txt`
4. Then run your project 
`python run.py`

✅ If everything runs smoothly, your `requirements.txt` is complete!
If not: install needed dependencies, test and then `pip freeze > requirements.txt`

✅ Now your project is fully reproducible for anyone who downloads it.

### Step 5: To delete `test_env`:
`deactivate`
`Remove-Item -Recurse -Force .\test_env` OR gitbash: `rm -rf test_env`

## Step 6: Create .gitignore for venv
This folder will not upload to github - important as venv is huge and useless to everyone else but your computer.

If in powershell: `New-Item .gitignore -ItemType File`
If in command prompt: `echo > .gitignore`
If gitbash: `touch .gitignore`

Then open .gitignore on VS Code or `code .gitignore` and type this in it and save:
```
# Ignore virtual environments
.venv/
test_env/
# Ignore OS files
.DS_Store
Thumbs.db
# Jupyter Notebook checkpoints
.ipynb_checkpoints
# Ignore Python cache
__pycache__/
*.pyc
```