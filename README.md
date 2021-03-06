# 后台管理系统模板
用来踩框架的坑。

## 目前支持的功能
* 左侧导航展开，合拢；根据路由高亮项目。
* 动态生成的面包屑。
* 多语言。用的 [vue-i18n](https://github.com/kazupon/vue-i18n) [doc](https://kazupon.github.io/vue-i18n/)。
* 对 Ajax 的封装。主要是用来处理通用错误。
* UI 组件
  * 带分页DataGrid 组件。支持排序，搜索等。
  * 信息提示框。 用的 [toastr](https://github.com/CodeSeven/toastr)
  * 下拉框。在 [select2](https://github.com/select2/select2) 上做的封装。
  * 日期选中框。在 [datetimepicker](http://xdsoft.net/jqplugins/datetimepicker/) 上做的封装。
  * 树形控件。在 [ztree](https://github.com/select2/select2) 上做的封装。
  * 展开合拢的渐变效果

## 运行
1. `npm i`
1. `npm run dev`
1. 在浏览器中输入地址 `127.0.0.1:5000`

## 构建
1. `npm run build`
1. 打开 `dist` 下的 `index.html`

## 用的主要的框架
* [Vue](http://vuejs.org/) 2.0
    * [vue-router](https://github.com/vuejs/vue-router) [doc](http://router.vuejs.org/zh-cn/index.html)
    * [vuex](https://github.com/vuejs/vuex) [doc](http://vuex.vuejs.org/en/index.html)。
    * [vue-resource](https://github.com/vuejs/vue-resource) [doc](https://github.com/vuejs/vue-resource/tree/master/docs)
    * [vue-i18n](https://github.com/kazupon/vue-i18n) [doc](https://kazupon.github.io/vue-i18n/) 多语言；国际化
* [Bootstrap](http://getbootstrap.com/) 3
* [PostCSS](http://postcss.org/)
  * [autoprefixer](https://github.com/postcss/autoprefixer)
* [Sass](http://sass-lang.com/)
* [Webpack](http://webpack.github.io/)
    * [vue-loader](http://vue-loader.vuejs.org/en/index.html)
    * [HTML Webpack Plugin](https://github.com/ampedandwired/html-webpack-plugin) 生成HTML。[HTML Webpack Template](https://github.com/jaketrent/html-webpack-template#html-webpack-template)
    * [extract text plugin for webpack](https://github.com/webpack/extract-text-webpack-plugin/blob/webpack-1/README.md) 将 Style 变成 独立成 link 标签。
* [Mock.js](http://mockjs.com/) 生成随机数据，拦截 Ajax 请求。

## 工具
* [vue-devtools](https://github.com/vuejs/vue-devtools)

## 参考
* [Vue Admin](https://github.com/fundon/vue-admin)
* [vue-smart-table](https://github.com/gurghet/vue-smart-table)
* [element](https://github.com/ElemeFE) 饿了么做的。
* [Awesome Vue.js](https://github.com/vuejs/awesome-vue)
* [vue-strap](https://github.com/yuche/vue-strap)