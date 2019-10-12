# cd 切換當前目錄至其它目錄

```

cd --help
cd: cd [-L|[-P [-e]] [-@]] [dir]
    Change the shell working directory.
    更改shell工作目录
    
    Change the current directory to DIR.  The default DIR is the value of the
    HOME shell variable.
    将當前目錄更改為DIR。默認的DIR是HOME shell變量的值
    
    The variable CDPATH defines the search path for the directory containing
    DIR.  Alternative directory names in CDPATH are separated by a colon (:).
    A null directory name is the same as the current directory.  If DIR begins
    with a slash (/), then CDPATH is not used.
    變量CDPATH定義包含DIR的目錄的搜索路徑。CDPATH中的其它目錄名由冒號分隔(:)。
    空目錄名與當前目錄相同。如果DIR以斜槓開頭，則不使用CDPATH。
    
    If the directory is not found, and the shell option `cdable_vars' is set,
    the word is assumed to be  a variable name.  If that variable has a value,
    its value is used for DIR.
    如果沒有找到目錄，並且設置了shell選項' cdable vars'，則假定該單詞是一個變量名。
    如果該變量有一个值，則將其值用於DIR。
    
    Options:
    設置:
      -L	force symbolic links to be followed: resolve symbolic
    		links in DIR after processing instances of 
            如果要切換的目標目錄是一個符號的連接，直接切換到字符連接名代表的目錄，而非符號連接所指向的目標目錄。
      -P	use the physical directory structure without following
    		symbolic links: resolve symbolic links in DIR before
    		processing instances of `..'
            如果要切換到的目標目錄是一個符號連接，直接切換到符號連接指向的目標目錄
      -e	if the -P option is supplied, and the current working
    		directory cannot be determined successfully, exit with
    		a non-zero status
            如果提供了-P選項，並且無法成功確定當前工作目錄，則以非零狀態退出
      -@	on systems that support it, present a file with extended
    		attributes as a directory containing the file attributes
            在支持它的系统上，將具有擴展屬性的文件顯示为包含文件屬性的目錄
    The default is to follow symbolic links, as if `-L' were specified.
    `..' is processed by removing the immediately previous pathname component
    back to a slash or the beginning of DIR.
    默認是跟随符號鏈接，就像指定了' -L'一樣。“. .通過將前一個路徑名组件删除回一个斜槓或DIR開頭來處理。
    
    Exit Status:
    退出狀態:
    Returns 0 if the directory is changed, and if $PWD is set successfully when
    -P is used; non-zero otherwise.
    如果目錄改變，返回0;如果使用-P成功設置$PWD，返回0;非零。


cd 進入用戶主目錄；
cd ~ 進入用戶主目錄；
cd - 返回進入此目錄之前所在的目錄；
cd .. 返回上級目錄（若當前目錄為“/“，則執行完後還在“/"；".."為上級目錄的意思）；
cd ../.. 返回上兩級目錄；
cd !$ 把上個命令的參數作為cd參數使用。

```
