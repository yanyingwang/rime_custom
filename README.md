rime_custom
======
为[Rime输入法](http://rime.im/)增加扩展词库并自定义Rime设置。


## 配置文件
* 双拼方案请见官方repo： https://github.com/rime/rime-double-pinyin


## 词库来源
* 拼音: https://github.com/Iorest/rime-setting/tree/158ee9d677d288a7354ce18aab02a97ff4ece5da
* 名郑码: https://github.com/yanyingwang/mzhengma


## 安装
首先不同系统的词库目标位置如下表：

| 系统   |    词库目录         |
|--------|---------------------|
| Linux - ibus  | ~/.config/ibus/rime <--> /usr/share/rime-data|
| Linux - fcitx | ~/.config/fcitx/rime |
| Mac OS | ~/Library/Rime      |
|Windows | %APPDATA%\Rime      |


以Linux系统的fcitx为例，执行如下命令删除rime的系统配置目录，并软连接本源目录到rime配置目录：

```shell
rm -rf ~/.config/fcitx/rime
ln -sf ~/rime_custom ~/.config/fcitx/rime
ls -ld ~/.config/fcitx/rime
```

然后重新部署，即可生效。



