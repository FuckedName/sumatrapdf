## SumatraPDF Reader

SumatraPDF is a multi-format (PDF, EPUB, MOBI, FB2, CHM, XPS, DjVu) reader
for Windows under (A)GPLv3 license, with some code under BSD license (see
AUTHORS).

More information:
* [main website](http://www.sumatrapdfreader.org) with downloads and documentation
* [manual](https://www.sumatrapdfreader.org/manual.html)
* [all other docs](https://www.sumatrapdfreader.org/docs/SumatraPDF-documentation-fed36a5624d443fe9f7be0e410ecd715.html)

To compile you need Visual Studio 2017. [Free Community edition](https://www.visualstudio.com/vs/community/) works.
I tend to update to the latest release of Visual Studio. Lately C++ evolves quickly
and Visual Studio constantly adds latest capabilities. If things don't compile,
first make sure you're using the latest update of Visual Studio.

To get the code:
* `git clone git@github.com:sumatrapdfreader/sumatrapdf.git`

Open `vs2017/SumatraPDF.sln` when using Visual Studio 2017


1、if use visual studio 2019 to compile
modify v140/v140_xp to v142 in vs2015/*.vcxproj files

2、error C2220: 警告被视为错误 - 没有生成“object”文件
点击项目，右击选择属性->配置属性->c/c++->常规，将“警告视为错误”的选项改为“否”。就可以！


[![Build status](https://ci.appveyor.com/api/projects/status/tesjtgmpy26uf8p7?svg=true)](https://ci.appveyor.com/project/kjk/sumatrapdf)
