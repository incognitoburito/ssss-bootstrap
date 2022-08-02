-When viewing the project or if you want to edit it.

1. Make sure git is install in your machine first
2. Bash should be where you’re at. if you haven’t installed node before (which should be the case to get this right)
3. Type: “touch ~/.bash_profile”
4. Type:
   curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
5. “kill” terminal (trash symbol) and restart another terminal. Make sure you are in correct folder.
6. Type: nvm install 16.13.2 (google newest nvm)
7. Type: nvm use 16.13.2 (just redo numbers)
8. Type: nvm alias default 16.13.2
9. Verify: node and npm is installed : node -v and npm -v
10. Create a package.json by typing: npm init Accept requirements

<---ignore below-----> 11. Install npm lite server: npm install lite-server –-save-dev
Npm lite server is a node.js based development web server. Basically a mock web server to use for testing development, not a real web server.

--save-dev flag means that lite-server is being installed as a development dependency, which means that later, when you build your project for deployment, it will not be included in the final build files, since it is only needed during development.

12. Modify package.json by opening file. Make sure main is in index.html
    Add this too:
    "scripts": {
    "lite": "lite-server",
    "start": "npm run lite",
    "test": "echo \"Error: no test specified\" && exit 1"
    },
