# kazuha-impression-maple-theme 枫原万叶印象主题 · 枫

## Preview (预览)
Preview image `images/preview.png`

click this >>> [Github](https://github.com/XiaoShi-studio/kazuha-impression-theme-maple/) <<<

![Preview](images/preview.png)

# English version
下有中文版
> A light VS Code theme based on the impression colors of Kaedehara Kazuha.

## Features
- 1. Use warm white (#fcf0e6) and similar colors as the main tone.
- 2. Use brown (#523532) and similar colors as interactive colors.
- 3. Use the color vermilion (#d13726) and similar hues as accents for interface elements.

## Instructions
After enabling the built-in AI agent feature (Settings -> Chat -> Other -> Disable AI Features: false), two buttons will appear on the right side of the Command Center: Switch Chat and a dropdown arrow.

At this point, the background color of the Command Center will be taken over by `agentStatusIndicator.background`, and `commandCenter.activeBackground` will no longer take effect. Both active and normal states will use `commandCenter.foreground` as the foreground color.

Now, let's look at the DOM structure of those two buttons:
(brief illustration)

```
<!--- This is the container controlling the two buttons --->
<div>
    <!--- This is the "Switch Chat" button --->
    <div></div>
    <!--- This is the dropdown arrow --->
    <div></div>
</div>
```
Since the hover state of this container (i.e., both buttons) is jointly controlled by `toolBar.hoverbackground`, and changing this would affect many other parts, there is no way to alter it.

That's the situation. So if you have the AI feature enabled, you will encounter the following:
- 1.The text in the Command Center becomes hard to read.
- 2.The hover effect on the two buttons malfunctions.
The author tried hard to find a satisfactory solution but ultimately couldn't, so it remains as is.
Thank you for your understanding!

## How to switch?
### 1. Direct Switch (Recommended):
- Select "Set Color Theme" above the interface

### 2.
- 1. Press <kbd>Ctrl</kbd> + <kbd>K</kbd>
- 2. Press <kbd>Ctrl</kbd> + <kbd>T</kbd> again
- 3. Select this topic in the pop-up options box

# Have fun!
### Developed by Xiaoshi

# 中文版
> 以枫原万叶印象色为基础的一款VS Code浅色主题。

## 特点
- 1.以 暖白色 (#fcf0e6) 及相近颜色为主色调。
- 2.以 棕褐色 (#523532) 及相近颜色为交互颜色。
- 3.以 朱红 (#d13726) 及相近颜色为界面元素点缀。

## 说明
在启用内置的AI智能体功能 (设置->聊天->其他->Disable AI Features: false) 后，命令中心右侧会出现两个按钮，**切换聊天**与一个下拉框箭头。

此时，命令中心的背景颜色将会被 `agentStatusIndicator.background` 接管，并且此时 `commandCenter.activeBackground` 失效，无论是active还是普通状态都将使用 `commandCenter.foreground` 作为前景色。

以及，让我们来看看那两个按钮的DOM结构：
(简洁示意)
```
<!---这是控制那两个按钮的容器--->
<div>
    <!---这是 切换聊天 按钮--->
    <div></div>
    <!---这是 下拉框箭头--->
    <div></div>
</div>
```
由于这个容器(即这两个按钮)的hover共同受 `toolBar.hoverbackground` 控制，因为此项牵一发而动全身，所以没有办法更改。

以上就是这些，所以如果您启用了AI功能，您将会遇到以下情况：
- 1.命令中心文字无法看清
- 2.两个按钮的悬停出故障

作者努力调试了很久，最后没能找到令我满意的方案，所以保留原样。
感谢您的理解！

## 如何切换？
### 1.直接切换 (推荐):
- 在界面上方选择 “设置颜色主题”

### 2.
- 1.按下 <kbd>Ctrl</kbd> + <kbd>K</kbd>
- 2.再按下 <kbd>Ctrl</kbd> + <kbd>T</kbd>
- 3.在弹出的选项框中选择本主题

# 玩得开心！
### 开发 by 小石
---
character designs © miHoYo/HoYoverse.
