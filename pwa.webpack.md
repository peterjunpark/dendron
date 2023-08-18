---
id: ac6b5yxsgbr1mxghl9zm8w9
title: Webpack
desc: ""
updated: 1692398226409
created: 1692395284092
---

Webpack is a popular open-source JavaScript module bundler that simplifies the management, bundling, and optimization of web assets. Using **loaders**, it takes various web assets such as JavaScript files, CSS stylesheets, images, and more, and intelligently bundles them together into one or more finely-tuned output files. This process is called **bundling**.

Out of the box, Webpack only bundles JavaScript files. To extend its prowess to other resources types, you must integrate a number of **loaders** and **plugins**.

Loaders, plugins, and other Webpack configurations live in the `webpack.config.js` file in the root directory of your project.

## Loaders

Loaders act as _transformers_ and _preprocessors_ that mold assets before they join the final production-grade bundle.

Each loader typically corresponds to an npm package that exports a function. When invoked, this function undertakes the necessary modifications to the assets, adapting them for inclusion in the bundle.

## Plugins

While loaders focus on individual files, plugins enhance Webpack's capability holistically. These supplementary modules operate on the complete bundle and orchestrate tasks like asset optimization, variable injection, code partitioning, and more.

Plugins are typically implemented as JavaScript classes tailored to specific actions.

## HMR

Webpack also encompasses a development server that serves the bundled files locally during development.

It also supports **hot module replacement** via the `HotModuleReplacementPlugin`, allowing you to see code changes in real-time, eliminating the need manually refresh the webpage and expediting development.

## Dist

By default, Webpack bundles all your assets and dependencies in the `src` directory and stores thde output into the `dist` directory.

When you run Webpack with a configuration, it reads the entry point(s) specified in the config file and recursively follows the dependencies of these entry points, creating a dependency graph. It then processes each module (file) in this graph using loaders and applies any necessary optimizations through plugins.

Typically, you'll find one or more JavaScript files, CSS files, and other assets in the `dist` directory--primed to be served to the client-side.

---

###### Resources

- https://webpack.js.org/guides/getting-started/
