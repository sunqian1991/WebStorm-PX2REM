## WebStorm-PX2RWD----px转rem/vw/vh插件

[![codebeat badge](https://codebeat.co/badges/290c72c6-f4e8-4f45-81e0-b98c612805b6)](https://codebeat.co/projects/github-com-sunqian1991-webstorm-px2rem-master)
[![](https://img.shields.io/badge/license-MIT-000000.svg)](https://github.com/sunqian1991/WebStorm-PX2REM/blob/master/LICENSE)
[![](https://img.shields.io/jetbrains/plugin/v/11187.svg)](https://plugins.jetbrains.com/plugin/11187-px2rem)
[![](https://img.shields.io/jetbrains/plugin/d/11187.svg)](https://plugins.jetbrains.com/plugin/11187-px2rem)
[![996.icu](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu)

#### 项目介绍

这是一个转换css文件中的px单位为rem/vw/vh等自适应设计页面（Responsive Web Design）单位的插件，主要适用于idea和webstorm. 

本项目参考了 https://github.com/yclnycl/ideapx2rem 中的代码，在他的基础上加入了一些新的功能。

如果有任何插件或开发相关的问题，欢迎跟我联系。

this is a tool of converting px to rem/vw/vh in a css/less file by a few settings.

#### 当前版本

V2.1.0

#### 更新日志

v2.1.0:添加了code intention和code completion；修改了配置页面的位置；修改了快捷键为<kbd>Alt</kbd> + <kbd>d</kbd>；

v2.0.2:在注释中添加了计算的过程；修改了保留小数位数的设置，在可以被整除的情况下，不改变精度

v2.0.1:添加了转换时精度与设置的比例相对应

v2.0.0:添加了转换整个文件的快捷键，修改了转换行内单位的逻辑；因转换文件的快捷键和默认的有冲突，现在将快捷键换成'shift d'和'ctrl shift d'

v1.1.5:添加了中文说明

v1.1.4:添加了英文说明

v1.1.3:处理了部分错误

v1.1.2:添加了用于转换比例值的持久化 

v1.1.1:修复了当前行内包含多条样式时无法转换的问题，将设置窗口移动到file-other settings下

v1.1.0:在原有的基础上添加了自动转换当前光标所在行中可以转换的值，将设置比值的窗口更改到tools菜单下，其中，需要注意行内不能包含多条样式；

v1.0.0:初始编写，webstorm插件，主要是把css中的px转换为rem，其中可以在webstorm中设置转化的比值(window-SetPX2REM),选中后通过快捷键shift+f来转化，如比值为100，选中"100px"后，点击shift+d，自动转化为1.00rem


v2.1.0: change the default short-cut key from shift + d to alt + d; add px to vw and px to vh; change the plugin-settings location to 'File - Settings - Px to Rwd'; add a code completion; add a code intention

v2.0.2: give a option of showing the calculation process in comment block; change the accuracy set

v2.0.1: change the accuracy set, which can be matched with the font size of root element

v2.0.0: give a short-cut key of ctrl + shift + d to convert the px to rem in a whole css file

v1.1.5: add some comments

v1.1.4: add some comments

v1.1.3: correct some errors

v1.1.2: add a persistence state of saving the custom settings

v1.1.1: correct some errors; change the setting location to 'File-Other settings'

v1.1.0: add a function of converting a line by short-cut key

v1.0.0: give a location to change the font size of root element


#### 联系我

如有任何问题，请联系我

QQ:991637393

email:sunqian1991@gmail.com


#### 使用说明

1. File - Settings - plugins - Browse repositories... - 搜索 'px2rem' - Install (也可以通过 File-Settings-plugins-install plugin from disk-选择生成的jar文件-restart webstorm 在本地安装).
2. File-Other Settings-PX2REM设置计算的比例值-选中代码段或光标移动到需要转换的行，点击shift+d.
3. 设置界面和快捷键设置可以在插件中自定义.
4. v2.0.0版本中加入了一键转换整个文件的功能，通过使用快捷键'ctrl shift d'来转换.
5. v2.0.2版本中加入了选择在注释中生成转换样式时的计算过程，在File-Other Settings-PX2REM选择勾选框可开启

there are three ways to convert: short-cut key, code intention, code completion. you can find the settings related to these converting ways in settings page with the path 'File - Settings - Px to Rwd'
 
1. short-cut key
 
select a converting type from three options of rem, vw, vh in setting page and give a necessary value set below the radio group, then use the default short-cut ket of Alt + d to convert a line or a selected text. you can also use the short-cut key of span style="color:#117ebf;font-weight: bold;">Ctrl + Alt + d to convert in a whole file.
you can only choose one converting type of short-cut key from rem,vw,vg to convert.
btw, you can change the short-cut key in your ide by setting the keymap option.
 
2. code intention
 
you can find three code intention types in settings page and you can select if a code intention type works by check the checkbox.
by check a code intention in a line of a css file, which will display by typing Alt + Shift, you can convert the line where the caret displays.
the unselected code intention types in settings page will not show in the list of code intention in a css file
 
3. code completion
 
you can also find three code completion types in the settings page and you can select if a code completion type works by check the checkbox.
by typing 'px' in a css file, you can find some code completion types you set in settings page. choose a type then it will give a result of converting.
the unselected code completion types in settings page will not show in the list of code completion in a css file
 
Instructions:
1. find menu at 'File - Settings - Px to Rwd', and give some settings.
2. select a text or move cursor at a line which contains a 'px' value.
3. use default shortcut key Alt + d to convert px to rem/vw/vh with a line; btw, you can change the shortcut at 'File - Settings - keymap - Plug-ins - px2rwd'.
4. use default shortcut key Ctrl + Shift d to convert px to rem/vw/vh with a file.
5. use a code intention to convert px to rem/vw/vh in a css file
5. use a code completion to convert px to rem/vw/vh in a css file

目前提供了三种方式来转换：快捷键、代码意图提示(Alt + Enter)、代码自动完成提示
 
1. 快捷键
 
默认的快捷键是Alt + d，在插件配置页面中可以看到快捷键部分有3种转换类型的选项，分别是rem,vw,vh，选择其中的一个来使用快捷键转换，需要注意的是，需要在选项下方的值配置中设置对应的基值。
只能选择一种转换类型来使用快捷键转换单位。同时也可以重新设置快捷键。需要注意的是，跟之前的版本相比，默认的快捷键修改了，修改的原因主要是原来的'Shift' + 'd'会与大小写冲突。
 
2. code intention
 
选择使用代码意图提示的类型后即可使用已选择的类型来在css文件中通过Alt + Shift来调用code intention来快捷转换单位。未勾选的选项不会出现在文件的code intention列表中。
 
3. code completion
 
选择使用代码自动提示的类型后即可使用已选择的类型来在css文件中快捷转换单位，当输入'px'后，code completion列表中会出现在配置页面中选择的类型名称，选择其中一个类型后即可实现自动完成转换功能。
 
如果觉得这个插件还不错，希望可以在github上给我点个赞，非常感激。
 
使用说明：
1. File-Settings-Px to Rwd进行必要的参数配置
2. 选择一个需要转换的样式或者将光标移动到一个包含需要转换样式的行中，使用快捷键Alt + d来转换，也可以使用Ctrl + Alt + d来转换整个文件中的可转换样式
3. 通过code intentionAlt + Enter来转换某一行中涉及到的样式
4. 通过在输入'px'字符后显示的自动完成提示列表中选择相应的选项来转换相应的样式


#### 注意事项
在使用插件转换时，**请避免在样式名称中使用值和`px`的组合**，如：
```css
.test200px{
    ...
}
```
此时`test200px`也会被自动转换，可能会造成极大风险

当启用在注释中显示计算过程的功能时，插件会在每次转换的样式的后面添加注释，在一些情况下会极大影响样式的可读性，请谨慎开启！！如：
```css
.test{
    box-shadow: 0.1rem    /* 10 / 100 */ 0.1rem    /* 10 / 100 */ 0.1rem    /* 10 / 100 */ #000;
    width:calc(100% - 0.2rem    /* 20 / 100 */);
}
```

![image][opt_gif]

#### 参与贡献

1. Fork 本项目
2. 新建 Feat_xxx 分支
3. 提交代码
4. 新建 Pull Request

本项目遵循MIT开源协议，代码当然可以被任意使用，同时也希望可以多多提交使用BUG和优化建议，如果能够pull request，那就太棒了！



[opt_gif]:https://github.com/sunqian1991/WebStorm-PX2REM/raw/dev/resources/option.gif
