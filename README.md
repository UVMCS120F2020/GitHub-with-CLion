# GitHub with CLion
We will be using GitHub for all of the Guided Projects, Open-Ended Projects, and the Final Project this semester. You should bookmark the organization page on your preferred web browser: [github.com/UVMCS120F2020](github.com/UVMCS120F2020)

GitHub stores a master copy of your project files, which you will be able to edit, add to, remove from, and track the history. It's kind of like Google Docs for code.

# Typical Files in a GitHub Repository
There are certain files that most GitHub repositories have:
* README.md is the file that opens automatically under the list of files on a repository page (like the one you're reading right now!). It uses markdown (which is what the .md file extenstion stands for) to write a description of the project, any installation instructions, or in the case of Guided Projects, directions to follow.
    * This file will be provided for you in Guided Projects, but you may need to edit it to answer questions.
    * You will need to create and populate this file for Open-Ended Projects and the Final Project.
    * The first time you open a README.md file in CLion, it will suggest you install a CLion markdown extension. I recommend it.
* .gitignore specifies all of the files and folders that exist in your project folder on your machine and which should not be in the GitHub repository. For the purposes of this course, this will include the folders that CLion creates to compile and run the project and store your IDE settings:
    ```asm
    cmake-build-debug/
    .idea/
    ```
  These two lines in the .gitignore file are very important, especially once you start collaborating on projects. This file will be provided for you in Guided Projects, but you will need to create it for Open-Ended Projects and your Final Project.
* Source files (those with .cpp and .h extensions) needed to run the project.
* In a larger project, you may have enough files to create folders for organization. For example, you may want a folder for all of your source files, one for images, and one for input and/or output data files.

# Cloning an Existing Project from GitHub to CLion
* Click the green "⤓ Code" button and copy the HTTPS link.
* You may need to install [Git](https://git-scm.com/downloads) on your machine.
* Now switch to CLion:
    * If you already have a project open in CLion, go to VCS -> Get from Version Control...
    * If you do not already have a project open in CLion, choose Get from Version Control from the main menu screen.
* In the window that pops up, choose Git from the dropdown menu.
* Paste the link from GitHub in the URL textbox.
* The Directory textbox is where CLion will create a folder for the project. Change it if the default directory is not where you want it.
* Click Clone.
    * You may be prompted to enter your GitHub username and password.
* It will ask you if you want to open the directory. Choose yes.
    * If you already have a project open in CLion, it will ask you if you want to open the project in a new window or this window. This choice is up to you.

# Creating a repository for an Open-Ended Project
* Go to the organization page on GitHub: [github.com/UVMCS120F2020](github.com/UVMCS120F2020)
* Click the green "New" button.
* The owner defaults to the organization. Do NOT change it.
* Choose a repository name, keeping with the required format in the Open-Ended Project directions.
* You can optionally provide a description for the project. This is what shows up when the repositories are listed in the organization. You can also edit/complete it later.
* The repository defaults to private. Do NOT change it.
* You can check the box to create a README file if you want. It will create a README.md file with the name of the repository and the description.
* There is a dropdown to add a .gitignore file. I do NOT recommend this. CLion has a setup different from other C++ projects, so I suggest you create your own .gitignore file once the repository exists.
* There is a dropdown to add a license. I do NOT recommend this.
* Click the green "Create Repository" button.
* Now follow the directions above to clone the repo into CLion.

# Mantra
* Work on the project. Add/modify files.
* When you finish a task, commit it and push it to the repository:
    * VCS -> Git -> Commit
    * Choose all files added/changed
    * Write commit message
    * Click the arrow in the "Commit" button and choose "Commit and Push"
    * Click "Push"
    * Wait for confirmation to appear in the lower right corner of CLion.
    
# CLion colors
CLion colors the text of the file names according to their git status:
* Black means the local file matches the one in the repository.
* Red means the file exists locally but is not in the repository.
* Green means the file is new and is ready to be pushed to the repository.
* Blue means the local file is different from the version in the repository (i.e. you made changes to the file that can be committed and pushed to the repository).
