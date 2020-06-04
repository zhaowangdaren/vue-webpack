# vue-webpack-skeleton

> 该工程模板基于[vuejs-templates/webpack](https://github.com/vuejs-templates/webpack)，在其基础上增加了骨架、vw适配

## 使用

``` bash
$ npm install -g vue-cli
$ vue init zhaowangdaren/vue-webpack-skeleton my-project
$ cd my-project
$ npm install
$ npm run dev
```

This will scaffold the project using the `master` branch. If you wish to use the latest version of the webpack template, do the following instead:

``` bash
$ vue init zhaowangdaren/vue-webpack-skeleton#develop my-project
```

:warning: **The develop branch is not considered stable and can contain bugs or not build at all, so use at your own risk.**

The development server will run on port 8080 by default. If that port is already in use on your machine, the next free port will be used.

### 编写骨架

在`src/Skeleton.vue`中编写骨架，不支持逻辑

## What's Included

- `npm run dev`: first-in-class development experience.
  - Webpack + `vue-loader` for single file Vue components.
  - State preserving hot-reload
  - State preserving compilation error overlay
  - Lint-on-save with ESLint
  - Source maps
  - 暂未支持骨架，在开发时可以通过路由的方式来开发骨架页面

- `npm run build`: 打包
  - 首先会运行`npm run skeleton`编译`src/Skeleton.vue`生成骨架
  - 运行`node skeleton.js`将渲染骨架内容，并将渲染后的骨架内容以index.html为模板写入`dist/index.html`
  - 打包业务逻辑

- `npm run unit`: Unit tests run in [JSDOM](https://github.com/tmpvar/jsdom) with [Jest](https://facebook.github.io/jest/), or in PhantomJS with Karma + Mocha + karma-webpack.
  - Supports ES2015+ in test files.
  - Easy mocking.

- `npm run e2e`: End-to-end tests with [Nightwatch](http://nightwatchjs.org/).
  - Run tests in multiple browsers in parallel.
  - Works with one command out of the box:
    - Selenium and chromedriver dependencies automatically handled.
    - Automatically spawns the Selenium server.

- `npm run skeleton`: 编译`src/Skeleton.vue`生成骨架

- 支持将px转换为vw，配置见`.postcssrc.js`

