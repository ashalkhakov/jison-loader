# Jison loader for webpack

## Usage

[Documentation: Using loaders](http://webpack.github.io/docs/using-loaders.html)

``` javascript
var parser = require("!raw!jison!./parser.jison");
// => returns compiled parser from parser.jison
```

### webpack config

``` javascript
module.exports = {
  module: {
    rules: [
      {
        test: /\.jison$/,
        use: "jison-loadere"
      }
    ]
  }
};
```

Then you only need to write: `require("./file.jison")`
