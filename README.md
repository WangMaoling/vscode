# feiyue

> A Vue.js project

项目不仅仅在web端显示，而且还会嵌入到肺悦2PC客户端，以及android客户端的肺悦云的webview里面，在PC客户端显示的时候有以下几点问题：
1.用到el-icon 字体图标的地方要注意，图标标签里面不可以放文字。
2.echarts折线图以及柱状图等显示的时候会错位，需要修改渲染方式为svg

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification 正式打包 打包根路径需要在 webpack.base.conf.js中设置
npm run build

# 测试环境打包  或者 命令：npm run build test
npm run build -- test

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).


项目中有5个组件用到版本处理分别是：
1.detail.vue //报告详情页面
2.subordinateDetail.vue //下级医院报告详情页面
3.diagnosis.vue //辅助诊断报告详情页面
4.subordinateDetail_blank.vue //远程会诊 患者的报告详情页面
5.print.vue //打印处理报告版本
