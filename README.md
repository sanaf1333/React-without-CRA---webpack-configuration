# React-without-CRA---webpack-configuration
Create react app without npx create-react-app with webpack configuration

1. Create an empty folder and open it in vs code
2. open terminal and write 
      npm init -y
3. run the following commands
npm install react
npm install react-dom
npm install webpack webpack-dev-server --save-dev
npm install @babel/core babel-loader @babel/preset-react @babel/preset-env --save-dev
npm install html-webpack-plugin
4. create a src folder and add index.js and index.html file
5. create a webpack.config.js file in your project and write the configurations given in the file above or whatever you want to configure it for
6. add following lines in "script" in package.json
"start": "webpack-dev-server --mode development --open --hot",
    "build": "webpack --mode production"
7. create a components folder in src, add app.js and write your code
8. run "npm start" to see your output
9. run "npm run build". It will create dist directory in your project (as configured in webpack.config.js) along with bundle.js.
