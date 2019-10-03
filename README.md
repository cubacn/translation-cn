[![license](https://img.shields.io/badge/license-Apache%20License%202.0-blue.svg?style=flat)](http://www.apache.org/licenses/LICENSE-2.0)

# CUBA中文翻译扩展组件

CUBA 平台的中文翻译（包含 BPM、Charts、Report、FTS），以扩展组件的方式开发

## 安装

**注意**: 该扩展组件的仓库已经托管至 CUBA 主仓库。可以直接通过 **CUBA Studio** 进行安装。

1. 安装：使用 CUBA Studio 打开项目。在左侧的 CUBA 项目树双击 `Add-ons` 或者使用主菜单的 `CUBA->Marketplace...` 选项打开扩展管理界面。
在打开的界面中选择 `Marketplace` 标签页，然后在搜索框输入 `chinese`，即可显示与当前 CUBA 版本兼容的中文包。然后点击 `INSTALL` 按钮
即可进行安装。

2. 更新：目前 Studio 已经支持自动更新组件，每次打开项目时，Studio 会自动检查组件更新。按照步骤操作即可。

3. 组件与平台版本的兼容性列表如下。注意，这里组件的版本描述（x.y.z）中，x.y 为平台版本，z 为中文组件版本。

|  平台版本  |  扩展组件版本  | 坐标
| ---------------- | -------------- | ------------
| 6.10.*           | 6.10.2         | cn.cuba.trans:transcn-global:6.10.2
| 7.0.*            | 7.0.2          | cn.cuba.trans:transcn-global:7.0.2
| 7.1.*            | 7.1.0          | cn.cuba.trans:transcn-global:7.1.0

4. CUBA 应用程序中添加中文语言支持：

使用 **CUBA Studio**，在左侧 CUBA 项目树，展开 `Project`，双击 `Properties` 在 `Available locales` 部分点击后面的小铅笔进行编辑，
弹窗中点击 `+` 号，添加新语言。Language 填 `中文简体`，注意中文的 Code 为 `zh_CN`。如果系统语言不是中文，需要在浏览器打开 CUBA 应用程序之后通过 Help->Settings->Language 进行选择。

系统语言设置与 CUBA 语言相关的注意事项请参考 CUBA 官方文档： https://doc.cuba-platform.cn/manual-7.1-chs/app_properties_reference.html#cuba.availableLocales 

需要注意的是：如果语言列表中没有跟用户操作系统语言相匹配的条目，那么 cuba.availableLocales 属性定义的语言列表的第一个语言将被用来作为默认语言。否则，即会选择跟用户操作系统语言相匹配的做为默认语言。

## 支持的数据库

_N/A_ - 该组件不需要任何数据库

## 创建的数据库表

_无_
