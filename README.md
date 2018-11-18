npm i -D --save babel-loader@next

babel-preset-env takes care of all es versions

mini-css-extract-plugin now replaces Extract-Text-Webpack-Plugin
under webpack.config, if you want access to file system, add:
``` 
  node: { 
    fs: 'empty'
  }
```

url-loader (can use file-loader instead): load images (can do inline)