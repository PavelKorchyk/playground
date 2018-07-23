# How to start a project

Setup
---
 
```
npm install
```

1. Create new folder with 'README.md' file and run 
```
git init
```
to start track your files.

2. Run
```
npm init -y
```
to create 'package.json' file and add '.gitignore' file with 'node_modules' line to do not track them.

3. Install Babel to use JSX.
```
    npm install --save babel-core
    npm install --save babel-preset-env
    npm install --save babel-preset-react
```
4. Add '.babelrc' file to configurate Babel and let it works with presets installed on the previous step.
 
```
{
    "presets": [
        ["env", { "modules": false }],
        "react"
    ]
}
```

5. Install Webpack with 
```
npm install --save webpack babel-loader
```

and add src/main.js, webpack.config.js files.


Compile
---
```
npm install webpack-command --save-dev
npm run compile
```
Usage
---
 
Start the development server with this command:
 
```
npm start
```