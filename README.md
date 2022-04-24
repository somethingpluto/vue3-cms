## Vue3CMS—vue3 后台管理系统

## 前言 😀

​ 这个项目是跟着 coderwhy 老师的 Vue3+Ts 课程的结业项目。在这长达 3 个月的时间，从 Vue2 过渡到了 Vue3+ts。本篇 blog 为对这个历时 1 个月项目的总结。

## 技术栈 🚧

·框架：Vue3+VueRouter+Vuex

·语言：TypeScript

·组件：ElementUI

## 展示 🏳‍🌈

​ 除 Overview 页面以外，其它页面主体均已完成。

gitee 仓库地址 👉：https://gitee.com/chx2333/fc_test_system

线上展示地址 👉：http://120.25.255.207/#/main/system/user

登录用户名：coderwhy 密码：123456

### 登录页面 🍕

![image-20220423192523630](https://xingqiu-tuchuang-1256524210.cos.ap-shanghai.myqcloud.com/1770/image-20220423192523630.png)

### 数据展示页面

![image-20220423192556552](https://xingqiu-tuchuang-1256524210.cos.ap-shanghai.myqcloud.com/1770/image-20220423192556552.png)

### 数据展示页面

![image-20220423192618060](https://xingqiu-tuchuang-1256524210.cos.ap-shanghai.myqcloud.com/1770/image-20220423192618060.png)

![image-20220423192633097](https://xingqiu-tuchuang-1256524210.cos.ap-shanghai.myqcloud.com/1770/image-20220423192633097.png)

### 表格数据操作页面

![image-20220423192757299](https://xingqiu-tuchuang-1256524210.cos.ap-shanghai.myqcloud.com/1770/image-20220423192757299.png)

## Get 到了啥？😀

### 项目的基本搭建

​ 除了脚手架的使用，还了解了各种其它配置的使用 eslint,husky 的使用

### 组件的抽取

​ 对于后台管理类前端应用，主要为数据的展示，可以通过对 UI 组件库里面的 Table 经行二次封装，通过 config 文件的形式，决定 Table 所要展示的内容。例如，数据展示页面，往往分为搜索页和数据展示页面。搜索页面可以通过在 config 指定 type 来实现不同输入框。数据展示页面，可通过插槽来实现不同的不同列的展示效果。

### UI 组件库的按需引入

​ UI 组件库的按需引入好处可以减小文件的大小。通过注册组件的函数，来实现需要用到哪一个组件引入哪一个组件。通过 app.Componet 方法注册数组里面已经定义的组件。

### 网络请求的处理

​ 网络请求，放在存储数据的地方，本次项目主要通过 Vuex 存储数据，网络请求也直接放在了 Vuex 中，页面需要时直接通过 Vuex 调用。
