---
{"dg-publish":true,"permalink":"/ζ Technique/Soft/Github/Github中英文说明切换/","title":"Github中README多种语言切换功能的实现","noteIcon":3,"created":"2025-03-09T09:27:12.619+08:00","updated":"2026-01-06T11:46:04.182+08:00"}
---

## Goal
Github中README多种语言切换功能的实现
## Scheme
在库文件中建立多个语言README.md文件，在README.md文件中设置跳转，可以使用如下面方式。
要点：
- ()中文件实际位置，示例不同语言的README.md放在根目录中，确保路径正确。
- 建议不通语种README.md放在根目录中，放在根目录文件夹中，切换语种会进入资源管理器模式。
```text
# README.md
列表样式：
- de_DE [Deutsch](README.de_DE.md)
- en [English](README.md)
- es_ES [Español](README.es_ES.md)
- fr_FR [Français](README.fr_FR.md)
- hy [Հայերեն](README.hy.md)
- pt_BR [Português do Brasil](README.pt_BR.md)
- ru [Русский](README.ru.md)
- sv_SE [Svenska](README.sv_SE.md)
- zh_CN [简体中文](README.zh_CN.md)
- zh_TW [繁体中文](README.zh_TW.md)
选项卡样式：
[English](README.md) | [简体中文](README.zh_CN.md) | [繁体中文](README.zh_TW.md)
```
效果如下：
## README.md
列表样式
- de_DE [Deutsch](readme/README.de_DE.md)
- en [English](θ%20Archive/Readme.md)
- es_ES [Español](readme/README.es_ES.md)
- fr_FR [Français](readme/README.fr_FR.md)
- hy [Հայերեն](readme/README.hy.md)
- pt_BR [Português do Brasil](readme/README.pt_BR.md)
- ru [Русский](readme/README.ru.md)
- sv_SE [Svenska](readme/README.sv_SE.md)
- zh_CN [简体中文](readme/README.zh_CN.md)
- zh_TW [繁体中文](readme/README.zh_TW.md)
选项卡样式
[English](θ%20Archive/Readme.md) | [简体中文](README.zh_CN.md) | [繁体中文](README.zh_TW.md)
注：选项卡样式在不同语种README.md取消该语种对用的地址更合理
## Reference
[参考](https://github.com/Win-Chin/TemplateBase)