# Ressources: 
https://www.kdnuggets.com/2023/04/stepbystep-guide-web-scraping-python-beautiful-soup.html

# Steps to set up the project locally and on github
1. Create folder
2. Create a requirements.txt file with all dependencies
3. Create virutalenv with anaconda: conda create --name webscraping_env python=3
4. Activate virtual environment: source activate webscraping_env
5. Install packages: pip install bs4, request OR
		     pip install -r requirements.txt
6. Initialise project with GitHub: git init
7. Create .gitignore file (list hidden files with ls -a): vim .gitignore, , esc-:wq, (nano .gitignore)

8. Push to git:
To link your local repository to your GitHub account and push your code to GitHub, you need to add a remote URL. Assuming you have already created a repository on GitHub, follow these steps:
	1. Create a new repository on GitHub (if you haven't already).
	2. Copy the repository URL (HTTPS or SSH)
	3. Terminal, navigate to the root directory of your project.
	4. Add the remote repository using the following command:
	 	git remote add origin https://github.com/anne-lene/webscraping.git
	5. Check: git remote -v
	6. Git add .
	7. Git commit "Initial commit"
	8. Push: git push -f origin main (branch name see git repo) (force push will ignore the gitignore file!), (WROKAROUND: Remove the to-be-ignored files on the GitHub and then add, commit, push again)

9. To revert to older branches on git, eg, accidentally deleted files, do:
	git log -> copy respective hash
	git checkout insert-hash insert-name-of-folder-to-be-reverted
	e.g. git checkout 13b01f7ca527f929af841bbdd1f85ddbf1f3a553 ./

# Webscraping



# Steps, when setting up the project on another system:
1. Clone the git repository: git clone <repository_url>
2. cd project
3. Create and activate the Anaconda environment:
	conda create --name webscraping_env python=3
	conda activate webscraping_env
4. Install the project dependencies: pip install -r requirements.txt 
	(conda install --file requirements.txt)

