# 0x00. Webpack

 webpack is a static module bundler for modern JavaScript applications. When webpack processes your application, it internally builds a dependency graph from one or more entry points and then combines every module your project needs into one or more bundles, which are static assets to serve your content from.

## Entry
An entry point indicates which module webpack should use to begin building out its internal dependency graph. Webpack will figure out which other modules and libraries that entry point depends on (directly and indirectly).

By default its value is ./src/index.js, but you can specify a different (or multiple) entry points by setting an entry property in the webpack configuration. For example:

webpack.config.js

module.exports = {
  entry: './path/to/my/entry/file.js',
};
