# Creating a New Project

To start, you'll navigate to the New Project page, either by clicking `New Project` on the Home Page, or going to File > New Project in the menubar.

## Name and Location

Once on the New Project page, there are several options available to you.
If you've already set a default folder in the [Preferences](preferences.md) page, the selected directory will be displayed on the left. If you haven't, or if you want this project in a different directory, you can update the file path with the `Choose Directory` button.

Below that, you'll name your project. snake_case is best practice, and spaces will automatically be replaced with an underscore. Be sure you've set a project name and the directory is set, you won't be able to proceed if this isn't done.

The complete project path is displayed below the project name input.

## Optional Settings

On the right are a list of optional settings. 

**Flask Project** - 
Flask projects will be created with blueprints and boilerplate files.

**Number of Blueprints** - If you're creating a Flask project, set how many blueprints you will need. (You can always add more manually if needed, once the project is created.) If you don't use blueprints, leave this as 0.

**Create Virtual Environment** - If enabled, pyStructify will create a virtual environment for you in your project's root folder.

**Virtual Environment Name** - If you've opted to include a virtual environment, this will be what it is named.

**Create Git Repo** - Only available if Git is installed on your computer. pyStructify will initialize the empty project directory as a git repo before creating the rest of the project structure.

**Create README.md** - Will create a README.md file in your projects root folder.

**Create requirements.txt** Will create a requirements.txt file, and allow you to select or list packages you want added to in on the next page.

**Install Requirements Upon Project Creation** - If checked, pyStructify will install your requirements (in your virtual environment if you've chosen to include one) once the project is created.

**Configure Environment Variables** - pyStructify will always generate a .env file for you with a randomly generated SECRET_KEY. If this box is checked, you will have the option to add additional environment variables on the next screen.

*Note: pyStructify does not store your environment variables. The information is cleared once the project is created or the program is exited.*

## Moving On

Once you're happy with your settings, click `Get Started!`

If you've checked the Flask Project box, you will be redirected to the [Flask configuration screen](flask-projects.md).

Otherwise, you will be redirected to the [General configuration screen](general-projects.md)