npm i -D --save babel-loader@next

babel-preset-env takes care of:
babel-preset-es2015
babel-preset-es2016
babel-preset-es2017
babel-preset-latest

mini-css-extract-plugin now replaces Extract-Text-Webpack-Plugin
under webpack.config, if you want access to file system, add:
``` 
  node: { 
    fs: 'empty'
  }
```
If using spread operators `npm i --save-dev @babel/plugin-proposal-object-rest-spread`

url-loader (can use file-loader instead): load images (can do inline)
css-loader is a fallback

If using heroku, use this script `"npm install --production && webpack -p"`

If using react-router don't forget to wrap the app with BrowserRouter