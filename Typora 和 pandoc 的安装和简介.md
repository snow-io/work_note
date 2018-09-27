## Typora 和 pandoc 的安装和简介

[TOC]

### Typora的安装

- [Typora安装地址](https://www.typora.io/)

- Themes的安装

  1. [Themes下载地址](https://theme.typora.io/)

  1. Themes安装方法

     > 1. Open preference panel from `File` → `Preference` from menubar, then click “Open Theme Folder”
     > 2. Copy css and related resources, like fonts or images, into the newly opened folder.
     > 3. Restart typora, then select it from `Themes` menu.

  ![](https://theme.typora.io/media/doc/install-theme/Snip20160921_2.png)

  1. 推荐使用 VUE 和 Barfi主题

### pandoc的安装与使用

- [pandoc安装地址](http://pandoc.org/installing.html)

- pandoc使用指南

  > ```
  > # 打开终端窗口，windows下打开cmd
  > # 小试牛刀，将input.txt文件转换为output.html文件。-o参数表示输出文件
  > pandoc -o output.html input.txt
  > 
  > -f: 指定输入格式，比如docx、epub、md、html等
  > -t: 指定输出格式，比如docx、epub、md、html等
  > -o: 输出到file文件
  > --verbost: 显示详细调试信息
  > --log： 指定输出日志信息
  > 
  > --list-input-formats：列出支持的输入格式。
  > --list-output-formats：列出支持的输出格式。
  > --list-extensions：列表支持Markdown扩展，后面跟一个+或者-说明是否在pandoc的Markdown中默认启用。
  > --list-highlight-languages:列出语法突出显示支持的语言。
  > --list-highlight-styles:列出支持语法高亮的样式。。
  > -v: 打印版本信息。
  > -h：显示语法帮助
  > 
  > # 一些例子
  > # 获取网页内容，并将其转换为markdown格式
  > pandoc -f html -t markdown http://www.fsf.org
  > 
  > # 将input.txt文件作为markdown输入，转换为latex
  > pandoc -f markdown -t latex input.txt
  > 
  > # 如果未指定-f、-t，pandoc则会根据输入文件输出文件的后缀来转换
  > pandoc input.txt -o output.pdf
  > 
  > # pandoc要求输入输出使用utf8编码，可以使用iconv命令进行编码转换
  > iconv -t utf-8 input.txt | pandoc | iconv -f utf-8
  > 
  > # 如果需要使用tex生成pdf文件，则需要下载latex编译器  
  > 
  > ---------------------
  > ```


