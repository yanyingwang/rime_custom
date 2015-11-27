
注意：此源已经不再维护，作者已转用[搜狗输入法](http://pinyin.sogou.com/linux/)
======



rime_custom
======
为[Rime输入法](http://rime.im/)增加扩展词库并自定义Rime设置。




## 安装rime

如您还未安装ibus-rime，请先执行如下命令安装：

    $ sudo aptitude install -y ibus-rime ibus-rime librime-data librime-data-double-pinyin librime-data-wubi



## 词库

从网络收集并整理了以下词库：

* [https://github.com/rime-aca/dictionaries](https://github.com/rime-aca/dictionaries)
* [https://github.com/daya-prac/Rime_custom_dict](https://github.com/daya-prac/Rime_custom_dict)
* [https://github.com/elxy/meow_mspy.git](https://github.com/elxy/meow_mspy.git)



## 新的输入法方案：小鹤迎双拼 - ying_flypy

与默认小鹤双拼相比：
* 支持英文单词词库
* 支持特殊输入符号和词组等，[见此文件](https://github.com/yanyingwang/rime_custom/blob/master/symbols.yaml)



## 自定义设置说明

* Rime输入法选单添加并且保留如下方案： 
  * 小鹤双拼
  * 朙月拼音
  * 五笔拼音
  * 英文单词
  * 日语假名
  * 小鹤迎双拼

<!--
**朙月拼音以及相关输入法默认启动英文输入模式**
-->



## 小鹤迎双拼截图

![list](https://raw.githubusercontent.com/yanyingwang/rime_custom/master/shotcuts/list.png)

![buuiwogjde](https://raw.githubusercontent.com/yanyingwang/rime_custom/master/shotcuts/buuiwogjde.png)

![!guitar](https://raw.githubusercontent.com/yanyingwang/rime_custom/master/shotcuts/guitar.png)

![!xz](https://raw.githubusercontent.com/yanyingwang/rime_custom/master/shotcuts/xz.png)

![!xzm](https://raw.githubusercontent.com/yanyingwang/rime_custom/master/shotcuts/xzm.png)

![!jm](https://raw.githubusercontent.com/yanyingwang/rime_custom/master/shotcuts/jm.png)




## 下载

    git clone https://github.com/yanyingwang/rime_custom_dict.git




## 安装词库和新的输入法方案：

将本源中的所有内容复制到Rime输入法相关的词库目录下，

以Linux系统为例：

    cp rime_custom_dict/*.yaml ~/.config/ibus/rime


不同系统的词库目标位置如下表：


| 系统   |    词库目录         |
|--------|---------------------|
| Linux  | ~/.config/ibus/rime |
| Mac OS | ~/Library/Rime      |
|Windows | %APPDATA%\Rime      |





## 变更词库名称

双拼使用者，请再将`double_pinyin.custom.yaml`文件重命名为您所使用的双拼方案名字，

以Linux系统和小鹤双拼为例：

    mv ~/.config/ibus/rime/double_pinyin.custom.yaml ~/.config/ibus/rime/double_pinyin_flypy.custom.yaml

双拼默认命名规则请参照下表：


| 輸入方案   | id                 |
|------------|--------------------|
| 自然码双拼 | double_pinyin      |
| 智能ABC双拼| double_pinyin_abc  |
| 小鹤双拼   | double_pinyin_flypy|
| MSPY双拼   | double_pinyin_mspy |




## 重新部署

重新部署，即可生效。


## ibus-rime状态栏icon消失

可执行如下命令替换原icon:

    $ cp icon/rime_custom/zhung-new.png /usr/share/ibus-rime/icons/zhung.svg


