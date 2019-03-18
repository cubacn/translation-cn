[![license](https://img.shields.io/badge/license-Apache%20License%202.0-blue.svg?style=flat)](http://www.apache.org/licenses/LICENSE-2.0)

# CUBA中文翻译扩展

CUBA 平台的中文翻译（包含商业组件），以扩展组件的方式开发

## 安装

**注意**: 该扩展组件的仓库已经官方链接到CUBA主仓库。

*可以直接跳到第二步，了解如何在CUBA项目中添加该组件。*，或者 *也可以选择* 将我们的仓库添加到项目的仓库列表。

1. [*可选*] 添加该 Maven 仓库 `https://dl.bintray.com/cubacn/cuba-trans-cn/` 至CUBA项目的 build.gradle 文件：

```
buildscript {
    
    //...
    
    repositories {
    
        // ...
    
        maven {
            url  "https://dl.bintray.com/cubacn/cuba-trans-cn/"
        }
    }
    
    // ...
}
```

或者，可以通过 **CUBA Studio** 来添加我们的仓库：在左侧CUBA项目，展开 `Project`，双击 `Properties`，在弹窗中，`Repositories` 部分点击 `+` 号，
在新打开的窗口中的 `URL` 输入 `https://dl.bintray.com/cubacn/cuba-trans-cn/`，然后点击 `OK`。 最后，选中刚才添加的仓库即可。

2. 选择一个能兼容项目平台版本的扩展组件版本：

|  平台版本  |  扩展组件版本  | 坐标
| ---------------- | -------------- | ------------
| 6.10.*           | 6.10.0          | cn.cuba.trans:transcn-global:6.10.0
| 7.0.*            | 7.0.0          | cn.cuba.trans:transcn-global:7.0.0

最新稳定版： `7.0.0`

在项目中添加自定义应用程序组件：使用 **CUBA Studio**，在左侧CUBA项目，展开 `Project`，双击 `Properties`，在弹窗中，
点击 `Custom components` 部分的 `+` 号。然后粘贴需要的版本坐标即可。

## 支持的数据库

_N/A_ - 该组件不需要任何数据库

## 创建的数据库表

_无_