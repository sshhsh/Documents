
xetex.bat 为 windows 系统下编译用的批处理文件，用的命令是 xelatex 编译两遍，如果出错则在第一遍后就停止。默认过滤输出信息只留下 error，能自动识别是否存在 bib 文件然后决定是否调用 bibtex。（还有一个如果编译成功则自动隐藏控制台的功能，后来我在 Sublime 内部实现了所以就注释掉了。）最后清理编译残余的中间文件。

Sublime 编辑器使用的编译配置文件 XeTeX.sublime-build，放到 sublime 的 User 文件夹即可。其它编辑器（偶只用过 notepad++ 和 Everedit…）是在编辑器内部设置绑定到 bat 文件即可。另外的 synctex.bat 和 dde.exe 是用来和 SumatraPDF 间进行 syntex 的。（Sublime 装上 LaTeXTools 插件即可，不需要这个）

Linux 下的 makefile 文件有热心童鞋分享[在这里](https://github.com/LePtC/LeNote/issues/2)。
