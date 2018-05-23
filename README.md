# 内网无法访问antd字体的解决方法

​		

## 简介

antd的Icon图标托管在[iconfont.cn](http://iconfont.cn/)上面，如果客户电脑无法访问公网，会出现图标无法显示的问题。

我们可以把字体文件下载到项目中，解决该问题。

​	

## 解决方法

​	

通过以下的地址下载字体文件

[下载地址](https://github.com/ant-design/antd-init/tree/master/examples/local-iconfont/iconfont)

​	

将4个字体文件添加到项目目录内，并编写以下css样式：

```css
@font-face {
  font-family: 'anticon';
  src: url('./font/iconfont.eot');
  src: url('./font/iconfont.eot?#iefix') format('embedded-opentype'),
    url('./font/iconfont.woff') format('woff'), 
    url('./font/iconfont.ttf') format('truetype'), 
    url('./font/iconfont.svg#iconfont') format('svg');
}
```

