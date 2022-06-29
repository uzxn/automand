﻿# Automand

## 快速开始

1. 编写命令文件（后缀名任意）
2. 命令行执行：`atm [command-file]`

## 命令行语法

`atm [command-file]`

## .atm 文件编写规范

1. 每行只有一个命令
2. 命令参数置于命令名称之后

## 命令列表

> 鼠标命令以 m 开头，键盘命令以 k 开头

| 命令名称 | 含义         |
| -------- | ------------ |
| `mleft`  | 按下鼠标左键 |
| `mright` | 按下鼠标右键 |
| `mmove`  | 增加鼠标坐标 |
| `kpress` | 按下键盘按键 |
| `wait`   | 等待一段时间 |

## 命令参数 & 范例

* `mleft`：按下鼠标左键
     * 参数：点击次数，每两次点击之间的时间（单位毫秒）
     * 范例：`mleft 10 100`
* `mright`：按下鼠标右键
     * 参数：点击次数，每两次点击之间的时间（单位毫秒）
     * 范例：`mright 10 100`
* `mmove`：增加鼠标坐标
     * 参数：增加的横坐标，增加的纵坐标（负数则减少）
     * 范例：`mmove 50 50`
* `kpress`：按下键盘按键
     * 参数：Virtual-Key 代码（见附录），点击次数
     * 范例：`kpress 65 10`
* `wait`：等待一段时间
     * 参数：时间（单位毫秒）
     * 范例：`wait 1000`

## 附录

* [Windows Virtual-Key](https://dwz.date/fmFy)：对应键盘上的按键
