## 概述

Win10 + [eclipse-jee-oxygen-R-win32-x86_64.zip](http://ftp.yzu.edu.tw/eclipse/technology/epp/downloads/release/oxygen/R/eclipse-java-oxygen-R-win32-x86_64.zip
) 实测通过。  
本文链接：<https://github.com/rj-hwang/ui-prototype-tools/tree/master/wireframesketcher/4.7.4>。  
下载地址：<https://pan.baidu.com/s/1mi0ycFA>  
WireframeSketcher 官方网站：<http://wireframesketcher.com>

## 安装步骤（含破解）

1. 解压到 eclipse 安装目录下的 dropins 子目录下。
    目录结构如下：  
    ```
    dropins
      |--wireframesketcher-4.7.4
           |--features
           |--plugins
    ```
2. 启动 Eclipse，然后点击菜单 Windows/Preferences>WireframeSketcher。  
    将会看到默认 15 天的试用期，如下图所示：  
    ![TrialExpiresIn14days](TrialExpiresIn14days.png)  
    注：首次启动并点击了上面的菜单后，将会自动在安装目录下生成文件 `configuration\.settings\com.wireframesketcher.ui.prefs`，内容如下：  
    ```
    eclipse.preferences.version=1
    location=0
    timestamp=1505351821225
    ```
    timestamp 的值是用来控制试用时间的，默认为 15 天的试用期（相对于 1970-01-01 之间的毫秒数）。
    直接把它改成 2023-01-01 对应的值 61633324800000，插件的 Status 就显示 Trial license，但不会提示几天后到期，相当于长期试用了，不过导出图片依然有水印。
3. 点击右下角的 "License Key..." 按钮执行注册。  
    填入 [LicenseKey.txt](LicenseKey.txt) 文件的内容，然后点击 "Register" 按钮返回后就可以看到注册成功的信息，如下图所示：  
    ![LicenseIsValid](LicenseIsValid.png)  
    此时文件 `configuration\.settings\com.wireframesketcher.ui.prefs` 内容如下：  
    ```
    eclipse.preferences.version=1
    licenseKey=---- BEGIN WIREFRAMESKETCHER KEY ---\r\nH4sIAAAAAAAAACXHuQ6CMAAG4L1PwW6MIp5D\r\nB7yCR03wQo0JqfpTaqRoW0R8ege/7YtjI4Xi\r\nttCIY8pG5Wg6DMW+1N3291VjIjJBmE2rJJ2c\r\nvrONn65nwWrxiR5MLNliVUb3+SA97LJB2N/7\r\nZ3qmJNEAVTmRxhQYcwva8hrNTqPVdNsk41JZ\r\nKK6uOIJrQ13P65FXwZWVtvpPQ0hjoXHb5vQi\r\nhavgJLl2/Df/BHkGYqsnKCseVtZ3BtpZyiuU\r\nwQ/9BcY9ygAAAA\=\=\r\n----- END WIREFRAMESKETCHER KEY ----\r\n
    location=0
    timestamp=1505351821225
    ```
    此时导出图片就没有水印了。
4. 首次接触 WireframeSketcher 的，可以打开其自带的教程例子快速上手。  
    自带教程例子打开方式：点击菜单 Help/Welcome>Tutorials>WireframeSketcher/Create a tutorial project。  
    更详细的语法请参考 [WireframeSketcher 官方帮助文档](http://wireframesketcher.com/help/help.html)。

## 其它

- [WireframeSketcher 官方帮助文档](http://wireframesketcher.com/help/help.html)
- [WireframeSketcher 官方网站](http://wireframesketcher.com)
- [Eclipse WireframeSketcher 插件安装地址](http://wireframesketcher.com/updates)： http://wireframesketcher.com/updates
