## 概述

Win10 + [eclipse-java-2021-12-R-win32-x86_64.zip](https://mirrors.nju.edu.cn/eclipse//technology/epp/downloads/release/2021-12/R/eclipse-java-2021-12-R-win32-x86_64.zip) 实测通过。  
![01-eclipse-4.22.0-202112](01-eclipse-4.22.0-202112.png)  
本文链接：<https://github.com/rj-hwang/ui-prototype-tools/tree/master/wireframesketcher/6.4.1>。  
下载地址：<https://pan.baidu.com/s/1BnEYF6x2ozkvXWJqoK51yA>  
WireframeSketcher 官方网站：<http://wireframesketcher.com>

> WireframeSketcher 6.4.1 release on 2021-12-17

## 安装步骤（含破解）

1. 解压到 eclipse 安装目录下的 dropins 子目录下。
    目录结构如下：  
    ```
    dropins
      |--wireframesketcher-6.4.1
           |--features
           |--plugins
    ```
2. 启动 Eclipse，然后点击菜单 Windows/Preferences>WireframeSketcher。  
    将会看到默认 15 天的试用期，如下图所示：  
    ![02-trial-expires-in-14days](02-trial-expires-in-14days.png)  
    注：首次启动并点击了上面的菜单后，将会自动在安装目录下生成文件 `configuration\.settings\com.wireframesketcher.ui.prefs`，内容如下：
    ```
    eclipse.preferences.version=1
    location=0
    timestamp=1640243026741
    
    ```
    timestamp 的值是用来控制试用时间的，默认为 15 天的试用期（相对于 1970-01-01 之间的毫秒数）。
    直接把它改成 2023-01-01 对应的值 61633324800000，插件的 Status 就显示 Trial license，但不会提示几天后到期，相当于长期试用了，不过导出图片依然有水印。  
    ![03-trial-expires-no-days](03-trial-expires-no-days.png)  
3. 点击右下角的 "License Key..." 按钮执行注册。  
    填入 LicenseKey.txt 文件的内容，然后点击 "Register" 按钮返回后就可以看到注册成功的信息，如下图所示：  
    ![04-license-valid](04-license-valid.png)  
    此时文件 `configuration\.settings\com.wireframesketcher.ui.prefs` 内容如下：
    ```
    eclipse.preferences.version=1
    licenseKey=---- BEGIN WIREFRAMESKETCHER KEY ---...----- END WIREFRAMESKETCHER KEY ----
    location=0
    timestamp=1640243026741

    ```
    此时导出图片就没有水印了。
4. 首次接触 WireframeSketcher 的，可以打开其自带的教程例子快速上手。  
    自带教程例子打开方式：点击菜单 Help/Welcome>Tutorials>WireframeSketcher/Create a tutorial project。  
    更详细的语法请参考 [WireframeSketcher 官方帮助文档](http://wireframesketcher.com/help/help.html)。

## 其它

- [WireframeSketcher 官方帮助文档](http://wireframesketcher.com/help/help.html)
- [WireframeSketcher 官方网站](http://wireframesketcher.com)
- [Eclipse WireframeSketcher 插件安装地址](http://wireframesketcher.com/updates)： http://wireframesketcher.com/updates


[破解来源]: https://www.zhinin.com/wireframesketcher-mac.html
