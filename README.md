# 五笔输入方案
可适配多平台的Rime配置方案。

## 声明
本项目引用了多个项目
- [极点五笔](https://github.com/KyleBing/rime-wubi86-jidian)。
- [五笔输入方案](https://github.com/rime/rime-wubi)。
- ~~[jieba词库](https://github.com/fxsjy/jieba)。~~
- 自制[五笔简码转换工具](https://github.com/x0710/HansConvertToWubi)，其中也引用了大佬们的项目内容。

本项目为自用极点魔改版本，当然你要是想再次魔改当然可以啦！

## 特色

上一个版本发现错误太多了
没有什么特别特色，后继再添加吧

> 妈妈再也不用担心我的打字速度

## 安装

### Linux

不同GNU/linx的配置目录略有不同，这里以[Arch Linux](https://wiki.archlinuxcn.org)为代表安装


1. 首先你要确保已经安装Rime框架，根据[Wiki](https://wiki.archlinuxcn.org/wiki/Rime)自行安装

2. 使用以下命令
```bash
git clone https://github.com/x0710/wb86.git
mkdir -p ~/.local/share/fcitx5/rime
mv wb86 ~/.local/share/fcitx5/rime # 假定你使用的是Fcitx5
```

3. 启动fcitx5，启用Rime，点击**Deploy**

### Android
> 同文安卓输入法 github：[https://github.com/osfans/trime](https://github.com/osfans/trime)  
> 输入法版本 release：[https://github.com/osfans/trime/releases](https://github.com/osfans/trime/releases)

下载本项目，解压后命名为`rime`，丢在系统根目录即可。

### 其它操作系统请参考极点官网配置
