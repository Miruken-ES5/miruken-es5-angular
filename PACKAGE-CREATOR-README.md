# Miruken Devs 
## Steps to publish to Bower & Yarn (npm):
1. Copy new files from dist folder of https://github.com/Miruken-ES5/miruken
2. `> yarn publish`  
	- (This uses the Miruken NPM Credentials) 
	- Tell it the new version. This will do 2 things: 
		1. Update package.json version  
		2. Create a commit with that version & tag it
3. IMPORTANT! Update bower.json version to match the one just updated in package.json
4. `> git commit --amend`  
	- (Save commit message without changing commit message)
5. `> git push`  
6. `> git push --tags`  
	- This will automatically create a bower version with that same version number

Voilà! That's it!