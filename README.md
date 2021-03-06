[![npm version](https://badge.fury.io/js/webpack-comment-remover-loader.svg)](https://badge.fury.io/js/webpack-comment-remover-loader)
# webpack-comment-remover-loader
A webpack loader that will remove JS comments from a file.

Uses [strip-json-comments](https://github.com/sindresorhus/strip-json-comments) to remove the comments.

## Loading JSON files which contain comments
Can be used with [json-loader](https://github.com/webpack/json-loader) to load json files which contain comments.

Example webpack config snippet:
```javascript
{
    test: /\.json$/,
    loaders: ['json-loader', 'webpack-comment-remover-loader'],
    exclude: /node_modules/
}
```
