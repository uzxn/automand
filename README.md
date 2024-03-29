# automand

Windows 自动化工具 命令行界面

## 快速开始

1. 编写命令文件 (后缀名任意)
2. 命令行执行: `atm [command-file]`

## 命令行语法

`atm [command-file]`

## 命令文件编写规范

1. 每行只有一个命令
2. 命令参数置于命令名称之后

## 命令列表 & 参数 & 范例

* `lu`: 松开鼠标左键
  * 无参数
* `ld`: 按下鼠标左键
  * 无参数
* `ln`: 点击鼠标左键若干次
  * 参数: 点击次数, 每两次点击之间的时间 (单位毫秒)
  * 范例: `ln 10 100`
* `ru`: 松开鼠标右键
  * 无参数
* `rd`: 按下鼠标右键
  * 无参数
* `rn`: 点击鼠标右键若干次
  * 参数: 点击次数, 每两次点击之间的时间 (单位毫秒)
  * 范例: `rn 10 100`
* `mv`: 移动鼠标 (增加坐标)
  * 参数: 增加的横坐标, 增加的纵坐标 (若为负数则减少)
  * 范例: `mv 50 50`
* `kb`: 点击键盘按键若干次
  * 参数: Virtual-Key 代码 (见附录), 点击次数
  * 范例: `kb 65 10`
* `wt`: 等待一段时间
  * 参数: 时间 (单位毫秒)
  * 范例: `wt 1000`

## 附录

* [Windows Virtual-Key Codes](https://docs.microsoft.com/en-us/windows/win32/inputdev/virtual-key-codes)
