# {{ name }}

> {{ description }}

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
{{#unit}}

# run unit tests
npm run unit
{{/unit}}
{{#e2e}}

# run e2e tests
npm run e2e
{{/e2e}}
{{#if_or unit e2e}}

# run all tests
npm test
{{/if_or}}
```
## 说明
# npm run build 命令 打包后生成文件在dist文件夹中，结构为springBoot项目定制可直接将dist内文件拷到springboot项目的resources文件夹下使用

# npm run dev 命令下 自动打开index.html页面

如需查看about页面请手动打开localhost:8080/about.html
8080为默认端口，根据自己实际更改
其他页面同理

在components 中添加通用组件

如需添加新页面请在pages中添加新文件夹并在其中添加同名.html文件，.js文件App.vue 等 参考index和about两个页面

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
