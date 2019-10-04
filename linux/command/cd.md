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
    
    Options:
      -L	force symbolic links to be followed: resolve symbolic
    		links in DIR after processing instances of `..'
      -P	use the physical directory structure without following
    		symbolic links: resolve symbolic links in DIR before
    		processing instances of `..'
      -e	if the -P option is supplied, and the current working
    		directory cannot be determined successfully, exit with
    		a non-zero status
      -@	on systems that support it, present a file with extended
    		attributes as a directory containing the file attributes
    
    The default is to follow symbolic links, as if `-L' were specified.
    `..' is processed by removing the immediately previous pathname component
    back to a slash or the beginning of DIR.
    
    Exit Status:
    Returns 0 if the directory is changed, and if $PWD is set successfully when
    -P is used; non-zero otherwise.


```
