# Tic Tac Toe Game

Learn GitHub Actions through a fun little game.

# Prettier

Add the Prettier format GitHub action from
https://mskelton.medium.com/auto-formatting-code-using-prettier-and-github-actions-ed458f58b7df

Add .prettierignore for ignoring files other than js

Add in package.json the command line ["format": "prettier --write ."] and fix the test format with npx standard **--fix**

Add workflows/node.js.yml the job


# Eslint 

https://medium.com/javascript-scene/streamline-code-reviews-with-eslint-prettier-6fb817a6b51d

Add the files for Eslint

Add in package.json the command line ["lint": "eslint --fix . && echo 'Lint complete.'"]

Add in workflows/node.js.yml the step for eslint


Add in .eslintrc  ["jest": true] for the test package
