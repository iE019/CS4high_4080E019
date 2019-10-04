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
  -E, --show-ends          display $ at end of each line
  -n, --number             number all output lines
      數字                 由1開始给所有輸出的行數編號
  -s, --squeeze-blank      suppress repeated empty output lines
  -t                       equivalent to -vT
  -T, --show-tabs          display TAB characters as ^I
  -u                       (ignored)
  -v, --show-nonprinting   use ^ and M- notation, except for LFD and TAB
      --help     display this help and exit
      --version  output version information and exit

Examples:
  cat f - g  Output f's contents, then standard input, then g's contents.
  cat        Copy standard input to standard output.

GNU coreutils online help: <https://www.gnu.org/software/coreutils/>
Full documentation at: <https://www.gnu.org/software/coreutils/cat>
or available locally via: info '(coreutils) cat invocation'


```
