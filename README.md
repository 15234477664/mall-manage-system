#### 1、项目整体结构

```makefile
mall-manage-system # 电商后台管理系统
|
---src
      |
      ---api
           |# axios实例 编写统一的请求响应拦截信息
            ---annotation
      ---assets # 存放静态资源和全局自定义样式
           |# 存放图片
            ---images 
           |# 存放自定义样式
            ---scss
      --- components # 小组件 一般这里的都是可以复用的
           |#首页侧边栏
            ---CommonAside.vue
           |#首页头部
            ---CommonHeader.vue
           |# element-ui 封装成公共from组件
            ---CommonForm.vue
           |# element-ui 面包屑组件
            ---CommonTab.vue
           |# element-ui 封装成公共表格组件
            ---CommonTable.vue 
           |# echarts 封装成公共图表组件
            ---EChart.vue  
        --- mock #模拟后端接口 返回数据
           |
        --- router#路由配置信息  
           |
        --- store #vuex配置信息
           |
        --- view # 页面级组件，一般复用性很低
           |# 首页相关组件
            ---Home
           |# 登陆页相关组件 
            ---Login
           |# 用户管理相关组件
            ---UserManage 
           |# 商品管理相关组件
            ---MallManage
           |# 主入口
            ---Main.vue
        --- App.vue
        --- main.js
        --- vue.config.js
```

#### 2、说明

接下来会分五篇博客大致讲下这个项目一些核心代码的实现

```
1、项目搭建+使⽤element实现⾸⻚布局
2、顶部导航菜单及与左侧导航联动的⾯包屑实现
3、封装一个ECharts组件的一点思路 
4、封装一个Form表单组件和Table表格组件 
5、企业开发之权限管理思路讲解
```


