# Preferences

When you first run the app, after the walkthrough, you'll be directed here to set a default directory.

You don't have to set one, but until one is set it will open to the Preferences page on startup.
*Note: Even with a default directory set, when you go to create a new project you have the option to update the directory it will be stored in.*

The Preferences page consists of two tabs, General and Flask.

## General

The General tab holds the default values of the options on the New Project screen. 

- **Default Project Directory** - The default directory projects will be created in (unless you update the directory on the new project screen)

- **Flask Project** - 
Flask projects will be created with blueprints and boilerplate files.

- **Number of Blueprints** - If you're creating a Flask project, set how many blueprints you will need. (You can always add more manually if needed, once the project is created.) If you don't use blueprints, leave this as 0.

- **Create Virtual Environment** - If enabled, pyStructify will create a virtual environment for you in your project's root folder.

- **Virtual Environment Name** - If you've opted to include a virtual environment, this will be what it is named.

- **Create Git Repo** - Only available if Git is installed on your computer. pyStructify will initialize the empty project directory as a git repo before creating the rest of the project structure.

- **Create README.md** - Will create a README.md file in your projects root folder.

- **Create requirements.txt** Will create a requirements.txt file, and allow you to select or list packages you want added to in on the next page.

- **Install Requirements Upon Project Creation** - If checked, pyStructify will install your requirements (in your virtual environment if you've chosen to include one) once the project is created.

- **Configure Environment Variables** - pyStructify will always generate a .env file for you with a randomly generated SECRET_KEY. If this box is checked, you will have the option to add additional environment variables on the next screen.

Updating values here stores them in pyStructify, so that when you navigate to New Project, it reflects the options you chose. Some are checked by default, but it's up to you to set it up exactly how you want it.

When you're happy with the settings you've chosen, click `Save Settings` at the bottom. *Note: If you navigate away from this page without saving, your changes will be lost.*
If you want to restore the default values, click `Restore Defaults`, below the save button.

*Note: The button to save the default directory is *not* the same as the save settings button. Once you've chosen a directory, a `Save` button will appear on the top right. This will update your directory settings. Anything else is handled with the bottom `Save Settings` button.

## Flask

Here is where you can setup the boilerplate for your Flask projects.

The defaults are set to the structure that I use with my Flask projects, including importing bootstrap 5.3 in `base.html`, importing packages in `__init__.py`, and setting up a User model in `models.py`. The files listed on the left are *not* the only files that will be generated, they are just the only ones configurable in pyStructify.

To begin editing the boilerplate, click the file you want to work on. This will open up an input on the right side of the screen, with the current default value. When you have finished making changes, click `Save`.

### IMPORTANT NOTES
- The `{project_name}` and `{bp}` placeholders will appear a couple times in the default code. Be cautious when making changes to these sections. It may cause your project to be created with code that doesn't run properly.
- You can use these placeholders wherever you need your project or blueprint names. *Note: the `{bp}` placeholder is only available in the two specified blueprint files.*
- The default values are stored as strings, so when using jinja syntax in `base.html` you need to add an extra pair of curly brackets `{}` around each one. Ex: in base.py the title is stored as `{{{{title}}}}`. This is to escape the escape sequence. So when it is written to your actual `base.html` file, it will just appear as `{{title}}`.
- In `__init__.py`, DO NOT update any code below `with app.app_context():`. This is how the blueprint imports and registrations are handled, and needs to be written this way for the project to work correctly. I included it in the input so if you know what you're doing and want to adjust the `__init__.py` boilerplate, you can see the full `create_app()` function. But editing the lines below the aforementioned one will result in your project not being created properly.

*Note: be sure to always click the `Save` button when updating the boilerplate. If you navigate away without saving, your changes will be lost.`

If you've removed the `with app.app_context()` line or you just want to remove any changes you added, scroll to the bottom and click the `Restore Defaults` button on the left. 

*Note: The tab you are on determines what defaults will be updated. If you want to update everything to the default, you will need to click `Restore Defaults` on both the Flask tab and the General tab.*