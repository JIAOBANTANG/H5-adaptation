# H5页面统一适配方案

- H5统一使用 `vw` 作为css长度单位
- H5兼容PC端统一使用 `rem` 作为css长度单位
- 网页应在 head 标签内添加 viewport meta 标签，以便优化在移动设备上的展示效果，其推荐的设置为：
~~~
<meta name="viewport" content="width=device-width, initial-scale=1">
~~~

## sass语法和安装方式
[推荐文章](https://laixiazheteng.com/article/page/id/ljjyDx1elX48)

## vs code配置
- 安装 Easy Sass 插件(ctrl+s 会直接编译为css文件)

## 使用方法
~~~
// 引入文件
@import 'reset.scss';
@import 'vw.scss';
//直接调用vw()函数即可,参数为设计稿元素实际像素大小
font-size:vw(72);
~~~

## 其他
- 移动端页面来说，通常会以`iPhone 7` 的分辨率（宽为 750 px）作为基准分辨率来出设计稿,其他分辨率请自行修改基准值
- 蓝湖设置平台为`web`，显示为像素单位即可;