# Flask Projects

The Flask Project screen consists of 2-4 tabs, depending on what settings you chose in the New Project screen.

## Blueprints
The first tab is where you'll name your blueprints. There will be a number of inputs equal to the number of blueprints you chose to include, or none, if you selected 0. Type the blueprint name(s) in, if applicable, then move on to the next tab.

## Packages

On the left is a list of commonly used packages. If you need anything that's not listed, simply type it into the box on the right.
Enter a new line between each item.

## Environment Variables

*Note: A SECRET_KEY is automatically included, you do not need to add that here.*
If you would like to add any additional environment variables, you can do that here. It should look like:

`VARIABLE="value"`

For example:

`MAIL_USERNAME="contact@aprilmaycodes.com"`

## Review
On the final tab you have the opportunity to review your project settings and structure before committing to it.

On the left, the settings you've chosen to (or not to) include will be listed, and below them the blueprints you've included, the packages that will be added to your requirements.txt, and the Environment Variables you've created.

If you need to make any changes, you can navigate to previous tabs and update them. 

To preview the project structure, click the `Preview Structure` button on the bottom left. This will open a display on the right side of the screen with your current project structure. The structure is the same for all Flask projects, with the exception of the optional files you selected on the New Project screen. If the project looks good to you, click the `Create Project` button.

A loading icon will be displayed while the project is being created, and then a popup window will appeat letting you know your project has been created. Once you close this popup, you'll be redirected to the home screen.
