# webpack-material-design-icons
Webpack Material Design Icons Font.
## Install
```bash
npm install --save-dev webpack-material-design-icons
```
## Usage
Just add `webpack-material-design-icons` to `entry.vendors` and handle the `png`, `woff`, `ttf` etc files in `webpack.config.js`
```JS
module.exports = {
    entry: {
        vendors: [
            "webpack-material-design-icons"
            ]
    },
    module: {
        loaders: [
        { test: /\.(jpe?g|png|gif|svg|eot|woff|ttf|svg|woff2)$/, loader: "file?name=[name].[ext]" }
        ]
    }
};
```
Of course you will need to configure how to handle CSS files as well.
## TODO
- Add working example.
