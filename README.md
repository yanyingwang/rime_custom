# rime_custom_dict



汇总网络中收集到的各种Rime输入法的词库


1.  下载词库 https://github.com/yanyingwang/rime_custom_dict.git (或是直接 clone / pull 這個 repo)

2.  将本源中的所有内容复制到Rime输入法相关的词库目录下：

~~~
# 词库目录：
# ~/.config/ibus/rime  (Linux)
# ~/Library/Rime  (Mac OS)
# %APPDATA%\Rime  (Windows)
~~~

3. 双拼使用者，请再将`double_pinyin.custom.yaml`文件重命名为您所使用的双拼方案名字，比如`double_pinyin_flypy.custom.yaml`，双拼默认命名规则请参照下表：


| 輸入方案   | id                 |
|------------|--------------------|
| 自然码双拼 | double_pinyin      |
| 智能ABC双拼| double_pinyin_abc  |
| 小鹤双拼   | double_pinyin_flypy|
| MSPY双拼   | double_pinyin_mspy |


