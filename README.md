# 软件的架构

## C/S(客户端/服务器)

* 一般我们使用的软件都是C/S架构的
* 比如系统中的软件
  * QQ
  * 微信
  * 等等
* C表示客户端
  * 用户通过客户端来使用软件
* S表示服务器
  * 服务器负责处理软件的业务逻辑
* 特点
  * 使用前必须安装
  * 软件更新时，服务器和客户端得同时更新
  * C/S架构的软件不能跨平台使用
  * C/S架构的软件客户端和服务器通信采用的是自有协议，相对来说比较安全。

## B/S(浏览器/服务器)

* B/S本质上也是C/S，只不过B/S架构的软件，使用浏览器作为软件的客户端
* B/S架构软件通过使用浏览器访问网页的形式，来使用软件
* 特点
  * 不需要安装，直接通过浏览器访问网页
  * 软件更新时，客户端不需要更新
  * 软件可以跨平台，只要系统中有浏览器，就可以使用
  * B/S架构的软件，客户端和服务器通信采用的是通用的HTTP协议，相对来说不安全
  * 可使用HTTPS安全的协议

## W3C标准

* 结构
  * HTML用于描述页面的结构
* 表现
  * CSS用于描述页面的样式
* 行为
  * JavaScript用于描述页面的行为

# HTML简介

* 超文本标记语言
* 它负责网页三要素中的结构
* 使用标签的形式来标识网页中的不同组成部分
* 所谓超文本指的是超链接，使用超链接可以让我们从一个页面跳转到另一个页面

## 标准格式
  ```html
  <!DOCTYPE html>
  <html lang="en">
  <head>
      <meta charset="UTF-8">
      <title>Document</title>
  </head>
  <body>

  </body>
  </html>
  ```

* `<!DOCTYPE html>`是文档声明
  * HTML4声明方式
    ```html
      <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
    ```
  * HTML5声明方式
    ```html
      <!DOCTYPE html>
    ```
  * XHTML声明方式
    ```html
      <?xml version="1.0" encoding="UTF-8"?>
      <!DOCTYPE html
        PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
        "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
    ```
  * 如果不写文档声明，则会导致有些浏览器进入怪异模式，浏览器解析页面无法正常显示

* `<html>`是根标签，有且只有一个，网页中的所有内容写在这个标签里面
* `<head>`标签用来设置网页的头部信息，不会在网页中直接显示，帮助浏览器解析网页
* `<body>`用来设置网页的主体内容，网页中所有可见的内容都写在body标签内
* `<title>`中的内容会显示在网页标题栏，搜索引擎在检索页面时会首先检索title中的内容，它是网页中对于搜索引擎来说最重要的内容，会影响到网页在搜索引擎中的排名
* `<meta charset="UTF-8">`是字符集声明