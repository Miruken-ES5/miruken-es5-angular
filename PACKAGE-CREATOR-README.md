# Miruken Devs 
## Steps to publish to Bower & Yarn (npm):
1. Copy new files from dist folder of https://github.com/Miruken-ES5/miruken
2. Update version in /bower.json to match the updated version from [https://github.com/Miruken-ES5/miruken/blob/master/lib/miruken.js](https://github.com/Miruken-ES5/miruken/blob/master/lib/miruken.js)
2. `> yarn publish`  
	- (This uses the Miruken NPM Credentials) 
	- When it prompts for new version, enter the same thing you changed it to in /bower.json (from [https://github.com/Miruken-ES5/miruken/blob/master/lib/miruken.js](https://github.com/Miruken-ES5/miruken/blob/master/lib/miruken.js)). This will do 2 things: 
		1. Update package.json version  
		2. Create a commit with that version & tag it
5. `> git push`  
6. `> git push --tags`  
	- This will automatically create a bower version with that modified version number

Voilà! That's it!