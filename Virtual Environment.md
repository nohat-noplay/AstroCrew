crtl-T for terminal
cd .. (to go up a folder)


https://www.geeksforgeeks.org/how-to-install-anaconda-on-ubuntu-20-04/
(Download Anaconda from https://docs.anaconda.com/anaconda/install/)

`conda info`
`conda update --all`

Make new directory for project
Create and manage an environment:
https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html

`conda create -n environment python`
`conda activate environment`
`conda list`
Install packages eg.
`pip install ipykernel` (for using virtual env)
`pip install numpy`


Export environment to environment.yml
conda env export > environment.yml
Look at yml from terminal `cat environment.yml`

When finishing on project for day or switching between projects:
`conda deactivate`


At end of project make requirements.txt file:
`pip freeze > requirements.txt`



How to replace a package with an older one inside the environment:
