# 安装
```
npm install scss-basic -D
```

## 使用vue-cli3及以上版本,全局使用该样式
创建vue.config.js
```
module.exports = {
  css: {
      loaderOptions: {
          //假设您已经安装了scss-basic，以及sass-loader、node-sass等
          sass: {
            prependData: `@import "~scss-basic";`
          }
      }
  }
}
```

> [参考文档](https://cli.vuejs.org/zh/guide/css.html#%E5%90%91%E9%A2%84%E5%A4%84%E7%90%86%E5%99%A8-loader-%E4%BC%A0%E9%80%92%E9%80%89%E9%A1%B9)

---
> 如若转载请注明出处