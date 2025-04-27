
1. Pull down from Github by going to desired Github folder in GitBash terminal (accessible from VS Code)

`git pull`

2. If want to create your own branch (Good for working on features or edits without affecting the main branch.)

`git branch mynewbranch`

check branch name is at end of your terminal name in brackets
Note: branch name should be applicable to what you are doing and/or your name

switch into that branch:

`git checkout mynewbranch`

(this is how you can switch back into main branch too if thats what you want)

If you need to update this branch from main, type in branch
`git merge main`

3. Once edited and saved your code - add to local git for that folder

`git add foldername.py` or add all changes `git add .`

4. Commit to local git

`git commit -m "meaningful comment"`

4. Push to github folder online into your branch

`git push origin mynewbranch`

5. Submit a pull request from your team to merge your branch into `main`: 
 - Go to [github.com](https://github.com)
 - Open your repo
- Click “Compare & pull request” & add  title and  description
- Click **“Create pull request”** to ask to merge your branch into `main`



