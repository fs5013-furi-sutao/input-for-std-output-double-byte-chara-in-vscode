# VSCode で全角で入力された文字を標準出力する方法

VSCode で Java プログラムを扱う際に、全角で入力された文字を標準出力する方法を説明する

## launcher.bat を開く

一度、Java ファイルを実行すると、次のように launcher.bat ファイルのパスが表示される。

![](./open_launcher_bat.png)



## launcher.bat を更新



laucher.bat
```bat
@echo off

REM Change code page to UTF-8 for better compatibility.
@chcp.com 932 > NUL 

REM Execute real command passed by args
%*

