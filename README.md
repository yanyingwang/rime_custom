rime_custom
======
自定义化的[Rime输入法](http://rime.im/)以及输入方案和词库。

官方文档请见:  https://github.com/rime/home/wiki/CustomizationGuide

## 快捷键
如果一个人要觉得一个软件好用，一定是建立在充分了解此软件的基础上的。<br>
比如快捷键，如果不够了解已有设计，就会觉得不顺手。Rime在快捷键的自定义上，提供的非常高的自由度，以下为我的自定义：
* 中英文的切换在Rime中完成：系统输入法一直停留在Rime上，完全的中文输入法和英文输入法的切换使用Rime中自定义的快捷键「Shift+Space」或「Ctrl+Shift+2」完成。
* 双拼输入时显示原始拼音：在使用双拼输入的时候，默认显示的是转码拼音（比如使用小鹤双拼输入xl显示的是xiang），此时按一下「Shift」按键会显示出原始编码（即xl），再按一次则恢复显示转码拼音（即xiang）。
* 支持Emacs风格的快捷键比如「Ctrl+N」、「Ctrl+P」等且非常好用。
* 使用「Ctrl+Shift+1」可在前两个中文输入方案之间来回切换。
* 使用「Ctrl+.」可来回切换使用中文符号或英文符号。


## 输入法方案
* 明月拼音：与朙月拼音相同，修改为简体显示。
* 小鹤双拼：https://github.com/rime/rime-double-pinyin
* 名郑码：https://github.com/yanyingwang/mzhengma


## 词库来源
* 拼音： https://github.com/Iorest/rime-setting/tree/158ee9d677d288a7354ce18aab02a97ff4ece5da
* 名郑码： https://github.com/yanyingwang/mzhengma
* 名语言函数名词库：http://www.yanying.wang/ming/

## 额外字符字体
名语言的词库包含一些自造字，其需要安装字体：https://github.com/yanyingwang/favfonts/tree/master/WenQuanWeiMiHeiExtend


## 安装
首先不同系统的词库目标位置如下表：

| 系统   |    词库目录         |
|--------|---------------------|
| Linux - fcitx5 | ~/.local/share/fcitx5/rime |
| Mac OS | ~/Library/Rime      |
|Windows | %APPDATA%\Rime      |


以Ubuntu 20.04系统的fcitx5为例（[需使用flatpak安装](https://www.yanying.wang/2022/11/how-to-run-fcitx5-and-rime-on-ubuntu-20-04.html)）:

```shell
cd ~/.local/share/fcitx5 &&\
rm -rf rime &&\
git clone https://github.com/yanyingwang/rime_custom rime &&\
ln -sf ~/.local/share/fcitx5/rime ~/rime_custom # for easily accessing configure directory of fcitx5-rime
```

然后重新部署，即可生效。

