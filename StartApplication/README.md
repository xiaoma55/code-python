# 一键批量打开应用

> 有时候开机之后，需要`打开很多应用`，尤其对我这种几乎每天需要带电脑回家的`打工人`。

> 那我们可以写个脚本`一键启动指定应用`。 

## 1 安装pyinstaller

```shell
pip install pyinstaller
```

## 2 打包

```shell
pyinstaller -F -w -i ./image/xiaoma.ico StartApplication.py
```

> 参数说明

```text
-F：打成单一文件
-w：关闭黑色框框，不然启动应用总会有个黑框框
-i：图标的位置
```

## 3 说明

> `打包完成`后，会在`StartApplication.py``同级目录`下生成`dist文件夹`，双击里面的`exe文件`就可以
> 启动脚本中指定的应用了，可以`右键把它添加到开始菜单`，这样就`方便`多了。

> `image`文件夹下`xiaoma.ico`是打包后的`exe文件图标`，可以自己替换，但是注意需要时`16*16`的`icon文件`，下面是我自己经常用的转icon的网站

[在线图片转icon](https://png2icojs.com/zh)
