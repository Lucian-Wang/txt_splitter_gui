# TXT 文本按行分割工具

基于 Python Tkinter，将 UTF-8 TXT 文件按指定行数分割。默认每份 1000 行，结果保存在输入文件所在目录，命名为 `原文件名_part1.txt`、`原文件名_part2.txt` 等。

## 安装与运行

```bash
git clone https://github.com/Lucian-Wang/txt_splitter_gui.git
cd txt_splitter_gui
python txt_splitter_gui.py
```

需要 Python 3 和 Tkinter；仅使用标准库，不需要 PyQt5 或压缩库，也没有 requirements.txt。旧二进制已移除，请按源码运行或自行打包。

## 使用

1. 点击“浏览”选择 TXT 文件。
2. 输入正整数，指定每个输出文件的行数。
3. 点击“开始分割”，查看完成提示。

目前只支持按行数分割，不支持按分隔符或压缩文件分割。程序会将整个文件读入内存；重复处理同名输入文件时，会覆盖已有同名分片。

## 许可说明

当前仓库未指定独立开源许可证。

## 维护与反馈

维护者：[Lucian](https://lucian.wang/) · 邮箱：im@lucian.wang · [问题反馈](https://github.com/Lucian-Wang/txt_splitter_gui/issues)
