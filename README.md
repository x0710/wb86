# 极点五笔
可适配多平台的Rime配置方案。
官方网站请点[这里](https://github.com/KyleBing/rime-wubi86-jidian)。

## 声明
这个项目引用了[jieba词库](https://github.com/fxsjy/jieba)，自制[五笔简码转换工具](https://github.com/x0710/HansConvertToWubi)，其中也引用了大佬们的项目内容。

本项目为自用极点魔改版本，当然你要是想再次魔改当然可以啦！

## 特色

- 主要在核心词库上采用了以词频为根据的权重，严格对照一级简码生成出的核心词库，让原极点词库更加充实。

- 单单一个核心词库即可应对绝大部分生活问题

- 接近于微软五笔词库？

但是由于严格按照词频排序，有些词汇，如`了`对应的一级简码为`b`，二级简码`bn`还是`了`，如果换成`也`会更好。
不过当前词库还处于试验期，后继会尝试加入严格二级简码。

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

### 文件说明
```bash
.
├── default.custom.yaml
├── FinalGodDict.dict.yaml          # 最终究极超级无敌大词典
├── LICENSE
├── lua
│   ├── wubi86_jidian_calculator.lua
│   └── wubi86_jidian_date_translator.lua
├── numbers.schema.yaml
├── README.md
├── wb86cutm.schema.yaml            # 仿极点五笔方案配置
└── 仓键盘布局
    └── wubi86_jidian_ios_keyboard.yaml
```
