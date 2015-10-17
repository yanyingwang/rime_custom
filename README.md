rime_custom_dict
======
汇总网络中收集到的各种Rime输入法的词库




## 1. 下载词库 

`git clone https://github.com/yanyingwang/rime_custom_dict.git`




## 2. 复制词库文件

将本源中的所有内容复制到Rime输入法相关的词库目录下，

以Linux系统为例：

`cp rime_custom_dict/*.yaml ~/.config/ibus/rime`


不同系统的词库目标位置如下表：


| 系统   |    词库目录         |
|--------|---------------------|
| Linux  | ~/.config/ibus/rime |
| Mac OS | ~/Library/Rime      |
|Windows | %APPDATA%\Rime      |





## 3. 变更词库名称

双拼使用者，请再将`double_pinyin.custom.yaml`文件重命名为您所使用的双拼方案名字，

以Linux系统和小鹤双拼为例：

`mv ~/.config/ibus/rime/double_pinyin.custom.yaml ~/.config/ibus/rime/double_pinyin_flypy.custom.yaml`

双拼默认命名规则请参照下表：


| 輸入方案   | id                 |
|------------|--------------------|
| 自然码双拼 | double_pinyin      |
| 智能ABC双拼| double_pinyin_abc  |
| 小鹤双拼   | double_pinyin_flypy|
| MSPY双拼   | double_pinyin_mspy |




## 4 . 重新部署

重新部署，即可生效。
