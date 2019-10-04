# pwd 用於顯示工作目錄

```

pwd --help
pwd: pwd [-LP]
    Print the name of the current working directory.
    打印當前工作目錄的名稱。
    Options:
    設置:
      -L	print the value of $PWD if it names the current working
    		directory
            如果$PWD指定了當前工作目錄，則打印它的值
      -P	print the physical directory, without any symbolic links
            打印物理目錄，不包含任何符號鏈接
    By default, `pwd' behaves as if `-L' were specified.
    默認情况下，' pwd'的行為就像' -L'被指定一样。
    Exit Status:
    退出狀態:
    Returns 0 unless an invalid option is given or the current directory
    cannot be read.
    返回0，除非给出了無效的選項或無法讀取當前目錄。

```
