# vue


复习ajax

mvc  路由  页面怎样渲染数据

Vue适合中小型项目
React适合大型项目

让网站往前排
SEO 搜索引擎优化
SEL 进价  

单页面：
    页面跳转：js渲染
    优点：页面切换快
    缺点：首屏事件稍慢 SEO差

多页面：


前端：如何进行组件化开发


### 前端发展史
- 黑铁时代 - 插件话  jquery
- 青铜时代  模块化  sea.js  require.js  ES6模块化
  模块：  
    防止冲突 ：解决命名冲突  变量冲突  函数名冲突  
    代码复用  
    解决依赖问题  
- 白银时代 - 组件化  
  组件化框架：react  vue
- 黄金时代 - 专业化
  组件库：ant element-ui

重点：SPA  组件

## 组件
简化开发的复杂度

核心思想：独立，完整，自由组合
-------------------------------------------
具备知识：
    - html+css
    - JavaScript （es5,es6,promise）  ajax  
    - node.js (服务器开发，前端工程化)


## vue
Vue是一个用于构建用户界面的框架
使用组件化方式开发单页面应用（SPA）

MVVM （model view view model） 双向视图绑定

### 兼容性
不支持IE9以下的浏览器


## vue基础语法
### 数据绑定

两种方式：
mustache：{{ 表达式 }}  
指令：v-bind 

mustache：{{ }}
    作用：
        取值
        运算
        调用函数或方法
        不可以进行for循环  定义函数等
指令：
    作用：
        取值
        运算
        调用函数或方法
        不可以进行for循环  定义函数等

## 指令
<h1 align="left"></h1>
<h1 align="left"></h1>

v-text
v-html
v-model  -> 只适用于表单  可以实现双向数据绑定 账号密码验证等信息的验证 可以通过user.username来调用

v-show  根据条件表达式的值来执行元素的隐藏或显示
v-if  根据条件表达式的值来决定元素是否添加或销毁
v-else if
v-else

v-for  遍历数组和对象  v-for=" (值,下标或字典的键) in lists"  表格  两层循环

v-once  数据绑定的时候只会在第一次进行修改

v-bind  动态绑定属性

v-on  绑定事件
    常用事件
        鼠标事件
            onclick indbclick
            onmouseover onmouseout
            onmouseenter onmouseleave
            onmousedown onmousemove onmouseup

        键盘事件
        窗口事件
        表单事件
        滚轮事件
    事件源.事件 = 事件处理程序

v-cloak  以隐藏未编译的 Mustache 标签直到实例准备完毕  在首屏第一页加载的时候写
    需要在css中设置[v-cloak]{display:none}
