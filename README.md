# demo template

## 简介

用于编写demo的模版，自带路由，方便管理和展示demo，依赖于[demobar](https://github.com/iwowen/demobar)

- demo地址 [https://iwowen.github.io/demobar/](https://iwowen.github.io/demobar/)
- demo地址2 [https://iwowen.github.io/demo-template/](https://iwowen.github.io/demo-template/)

## 使用

1. 首先下载项目，或者`fork`中后克隆自己的项目。

```shell
git clone https://github.com/iwowen/demo-template.git --recursive
```

2. 然后初始化项目，运行

```shell
npm run init //不是 npm init
npm run serve
```

3. 在`src`目录下开发demo，需要创建目录结构`src/{分类}/{demo名称}`。

## 更新 demobar

在项目根目录下运行
```shell
git submodule foreach git pull
```
或
```shell
cd demobar
git pull
```

## 主题

项目通过`config.js`配置主题，默认为`default`主题。
可以开发新的主题放在`theme`目录下，然后修改`config.js`中`theme`配置。

## 打包和部署

在根目录运行`npm run build`，项目将打包到`docs`目录。
之后可以在`github`中部署`gitpage`页面。

## 截图

![demo](https://raw.githubusercontent.com/iwowen/demo-template/main/screenshot/20210107172645.jpg "demo主页")
