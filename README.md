
# 1、uni-app是一个使用vue.js开发所有前端应用的框架，实现了一套代码，同时运行到多个平台

# 2、页面构成
## pages配置:接收数组，里面有path路径和style，相应的页面新增和添加的主文件管理
## tabBar应用:主要是list、text;最少2个，最多5个

# 3、生命周期
## 应用生命周期：app.vue主组件，调用应用生命周期函数、配置全局样式、配置全局的存储；
## 页面生命周期：每个页面也有周期
## 组件生命周期：

# 4、组件
## 基础组件
### view 视图容器，用来包裹其他真正显示的组件；类似div,用于包裹各种元素内容;
#### 属性 hover-class:点击出现的效果；hover-stop-propagation：阻止冒泡
### scroll-view 区域滚动容器；
#### 属性 scroll-x 横向滚动；scroll-y 纵向滚动

# 5、编译：
## 条件编译，在编译时根据这些特殊的注释，将注释里面的代码编译到不同平台

# 6、页面和路由
## 主要是页面跳转
### uni.navigateTo 保留当前页面，跳转到应用内的某个页面，使用uni.navigateBack
### uni.redirectTo 关闭当前页面，跳转到应用内的某个页面。
### uni.switchTab 跳转到tabBar页面，并关闭其他所有非tabBar页面

# 7、数据缓存:浏览器的localStorage
## 存储：uni.setStorage
## 获取：uni.getStorage
## 移除：uni.removeStorage

# 8、网络
## uni.request 请求数据；H5会有跨域，小程序没问题；前端解决方法：后端接收数据：fiel_get_content('php://input')
## uni.chooseImage 上传; uni.previewImage 预览；uni.getImageInfo 获取上传的图片信息

# 9、下拉刷新和上拉加载

# 10、自定义组件

# 11、打包编译




















