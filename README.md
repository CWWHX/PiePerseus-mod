# **Perseus**

本项目来自于[https://github.com/4pii4/PiePerseus](https://github.com/4pii4/PiePerseus)，更原始的项目为[https://github.com/Egoistically/Perseus](https://github.com/Egoistically/Perseus)。

用于修改《碧蓝航线》，实现简单的开挂（***注意封禁！禁止修改涉及活动EX、META作战、META支援、共斗等部分的数据***）。

## 配置

设置文件 `Perseus.json` 位于游戏的外部文件目录中（`/sdcard/Android/data/{package-name}/files/`）。

## ***<u>配置文件中文注释（中文环境下建议先看中文注释！！！）</u>*** 

[中文注释](https://github.com/CWWHX/PiePerseus-mod/blob/main/README_%E4%B8%AD%E6%96%87%E6%B3%A8%E9%87%8A.md)

## 功能（在原Perseus的基础上）：

* [X] 使用 `json` 格式的配置文件
* [X] 聊天框内可以使用一些命令
* [X] 移除低心情警告
* [X] 自定义自动重复次数（部分场景无效）
* [X] 跳过战列舰开火动画
* [X] 隐藏背景图片（没啥大作用）
* [X] 移除困难模式的部分限制

  * [X] 移除困难模式的全部限制
* [X] 指挥官信息伪装（自慰）
* [X] ~~任何科研船蓝图可分解~~（删掉了这个功能，这个会导致账号登录的时候闪退，后续再测试）
* [X] 增加大世界快速移动
* [ ] 增加建造彩、金的概率（想屁吃）


## 加载库

在 `UnityPlayerActivity` 中添加以下代码，放在 `onCreate` 的任意位置即可：

```smali
.method private static native init(Landroid/content/Context;)V
.end method
```

并在 `onCreate` 中添加以下代码：

```smali
const-string v0, "Perseus"

invoke-static {v0}, Ljava/lang/System;->loadLibrary(Ljava/lang/String;)V

invoke-static {p0}, Lcom/unity3d/player/UnityPlayerActivity;->init(Landroid/content/Context;)V
```

（最好在不替换其他变量的情况下添加，例如在 `.locals 2` 和 `const/4 v0, 0x1` 之间。）

**然后在lib中添加Perseus的so文件。**



## 感谢

[@Egoistically](https://github.com/Egoistically)

[@4pii4](https://github.com/4pii4)
