Using babel-loader^8beta `npm i --save-dev babel-loader@next` to avoid webpack confusing which babel to use.

If using spread operators `npm i --save-dev @babel/plugin-proposal-object-rest-spread`

babel-preset-env takes care of:
- babel-preset-es2015
- babel-preset-es2016
- babel-preset-es2017
- babel-preset-latest

Mini-CSS-Extract-Plugin now replaces Extract-Text-Webpack-Plugin (deprecated).

If you want access to file system, add under webpack.config:
``` 
  node: { 
    fs: 'empty'
  }
```

url-loader (can use file-loader instead): load images (can do inline).

css-loader is a fallback.

If using react-router don't forget to wrap the app with BrowserRouter

If using heroku, use this script `"npm install --production && webpack -p"`

If using express, don't forget to switch entrypoint in webpack.