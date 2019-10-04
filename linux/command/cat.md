# cat 用於連結文件並打印到標準輸出設備上

```

cat --help
Usage: cat [OPTION]... [FILE]...
用法:cat[选项]…[文件]…
Concatenate FILE(s) to standard output.
將文件連接到標準输出。

With no FILE, or when FILE is -, read standard input.
如果沒有文件，或者當文件为-时，讀取標準输入。

  -A, --show-all           equivalent to -vET
      全部顯示              相當於 -vET
  -b, --number-nonblank    number nonempty output lines, overrides -n
      數字-非空的           和-n相似，只不過對於空白行不編號
  -e                       equivalent to -vE
                           相當於 -vE
  -E, --show-ends          display $ at end of each line
                           在每行的末尾顯示$
  -n, --number             number all output lines
      數字編號              由1開始给所有輸出的行數編號
  -s, --squeeze-blank      suppress repeated empty output lines
                           禁止重复的空输出行
  -t                       equivalent to -vT
                           相當於 -vT
  -T, --show-tabs          display TAB characters as ^I
                           顯示制表符为^I
  -u                       (ignored)
  -v, --show-nonprinting   use ^ and M- notation, except for LFD and TAB
      顯示非打印使用^和M-符号，除了LFD和制表符
      --help     display this help and exit
      帮助       显示此帮助并退出
      --version  output version information and exit
      版本       輸出版本信息並退出。
Examples:
例子:
  cat f - g  Output f's contents, then standard input, then g's contents.
             輸出f的內容，然後是標準輸入，然後是g的內容。
  cat        Copy standard input to standard output.
             將標準輸入複製到標準輸出。
GNU coreutils online help: <https://www.gnu.org/software/coreutils/>
Full documentation at: <https://www.gnu.org/software/coreutils/cat>
or available locally via: info '(coreutils) cat invocation'


```
