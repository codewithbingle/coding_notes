Bootstrap

Initial Set-up
When starting to build you project, you need to go to the Bootstrap website and link it to your html.

On your terminal, you need to "npm init"
Next, npm i date-fns (this is optional)
Next, npm install bootstrap
Next, npm install lite server " npm install lite-server --save-dev " (not of production use)
---on your package.json file, do this
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "start": "npm run lite", (this must me added)
    "lite": "lite-server" (this must be added)
  },
