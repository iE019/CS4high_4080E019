# ls 用於顯示指定工作目錄下之内容（列出目前工作目錄所含之文件及子目錄)。

```
ls --help
Usage: ls [OPTION]... [FILE]...
List information about the FILEs (the current directory by default).
Sort entries alphabetically if none of -cftuvSUX nor --sort is specified.

Mandatory arguments to long options are mandatory for short options too.
  -a, --all                  do not ignore entries starting with .
  顯示所有文件及目錄 (ls內定將文件名或目錄名稱開頭為"."的視為隱藏檔，不會列出)
  -A, --almost-all           do not list implied . and ..
  同 -a ，但不列出 "." (目前目錄) 及 ".." (父目錄)
      --author               with -l, print the author of each file
                             使用-l，打印每个文件的作者
  -b, --escape               print C-style escapes for nongraphic characters
                            將文件中的不可輸出的字符以反斜線“”加字符編碼的方式輸出；
      --block-size=SIZE      with -l, scale sizes by SIZE when printing them;
                               e.g., '--block-size=M'; see SIZE format below                          
  -B, --ignore-backups       do not list implied entries ending with ~
                             不要列出以?结尾的隐含条目
  -c                         with -lt: sort by, and show, ctime (time of last
                               modification of file status information);
                               with -l: show ctime and sort by name;
                               otherwise: sort by ctime, newest first
   與“-lt”選項連用時，按照文件狀態時間排序輸出目錄內容，排序的依據是文件的索引節點中的ctime字段。
   與“-l”選項連用時，則排序的一句是文件的狀態改變時間；                            
  -C                         list entries by columns
      --color[=WHEN]         colorize the output; WHEN can be 'always' (default
                               if omitted), 'auto', or 'never'; more info below
  -d, --directory            list directories themselves, not their contents
                            僅顯示目錄名，而不顯示目錄下的內容列表。顯示符號鏈接文件本身，
                            而不顯示其所指向的目錄列表；
  -D, --dired                generate output designed for Emacs' dired mode
                            生成為Emacs dired模式設計的輸出
  -f                         do not sort, enable -aU, disable -ls --color
                            此參數的效果和同時指定“aU”參數相同，並關閉“lst”參數的效果；
  -F, --classify             append indicator (one of */=>@|) to entries
      --file-type            likewise, except do not append '*'
      --format=WORD          across -x, commas -m, horizontal -x, long -l,
                               single-column -1, verbose -l, vertical -C
      --full-time            like -l --time-style=full-iso
      在每個輸出項後追加文件的類型標識符，具體含義：“*”表示具有可執行權限的普通文件，“/”表示目錄，
      “@”表示符號鏈接，“|”表示命令管道FIFO，“=”表示sockets套接字。當文件為普通文件時，不輸出任何標識符；
  -g                         like -l, but do not list owner
      --group-directories-first
                             group directories before files;
                             文件之前的组目录
                               can be augmented with a --sort option, but any
                               use of --sort=none (-U) disables grouping
                              可以使用——sort选项进行扩展，但是使用——sort=none (-U)会禁用分组
  -G, --no-group             in a long listing, don't print group names
                             在長列表中，不要打印组名
  -h, --human-readable       with -l and -s, print sizes like 1K 234M 2G etc.
                             具有-l和-s，打印尺寸为1K 234M 2G等。
      --si                   likewise, but use powers of 1000 not 1024
                             同樣的，使用1000的幂而不是1024
  -H, --dereference-command-line
                             follow symbolic links listed on the command line
                             遵循命令行中列出的符号链接
      --dereference-command-line-symlink-to-dir
                             follow each command line symbolic link
                             遵循每個命令行符號链接
                               that points to a directory
                               它指向一个目录
      --hide=PATTERN         do not list implied entries matching shell PATTERN
                               (overridden by -a or -A)
                             不要列出与shell模式匹配的隐含项(被-a或-a覆盖)
      --hyperlink[=WHEN]     hyperlink file names; WHEN can be 'always'
                               (default if omitted), 'auto', or 'never'
                               超链接文件名稱;WHEN可以是'always'(省略時默認)、'auto'或'never'
      --indicator-style=WORD  append indicator with style WORD to entry names:
                               none (default), slash (-p),
                               file-type (--file-type), classify (-F)
                             将带有样式词的指示符附加到条目名称:none(默认)、slash (-p)、
                             file-type(—file-type)、classification (-F)
  -i, --inode                print the index number of each file
   顯示文件索引節點號（inode）。一個索引節點代表一個文件；
  -I, --ignore=PATTERN       do not list implied entries matching shell PATTERN
  -k, --kibibytes            default to 1024-byte blocks for disk usage;
                             以KB（千字節）為單位顯示文件大小；
                               used only with -s and per directory totals
                               僅用於-s和每個目錄彙總
  -l                         use a long listing format
                             除文件名稱外，亦將文件型態、權限、擁有者、文件大小等資訊詳细列出
  -L, --dereference          when showing file information for a symbolic
                               link, show information for the file the link
                               references rather than for the link itself
  -m                         fill width with a comma separated list of entries
                             用“,”號區隔每個文件和目錄的名稱；
  -n, --numeric-uid-gid      like -l, but list numeric user and group IDs
                             以用戶識別碼和群組識別碼替代其名稱；
  -N, --literal              print entry names without quoting
                             打印条目名稱，不带引號
  -o                         like -l, but do not list group information
                             類似-l，但不要列出组信息  
  -p, --indicator-style=slash
                             append / indicator to directories
                             添加/指标目录
  -q, --hide-control-chars   print ? instead of nongraphic characters
                             打印?而不是非图形字符
      --show-control-chars   show nongraphic characters as-is (the default,
                               unless program is 'ls' and output is a terminal)
                             按原样显示非图形字符(默认，除非程序是“ls”，输出是终端)
  -Q, --quote-name           enclose entry names in double quotes
                             將條目名稱放在双引号中
      --quoting-style=WORD   use quoting style WORD for entry names:
                              对条目名称使用引用样式词
                               literal, locale, shell, shell-always,
                               文字，语言环境，shell，总是shell
                               shell-escape, shell-escape-always, c, escape
                               (overrides QUOTING_STYLE environment variable)
                              shell-escape、shell-escape-always、c、escape
                              (覆盖引用样式环境变量)
  -r, --reverse              reverse order while sorting
                             以文件名反序排列並輸出目錄內容列表；
  -R, --recursive            list subdirectories recursively
                             遞歸處理，將指定目錄下的所有文件及子目錄一併處理；
  -s, --size                 print the allocated size of each file, in blocks
                             顯示文件和目錄的大小，以區塊為單位；
  -S                         sort by file size, largest first
      --sort=WORD            sort by WORD instead of name: none (-U), size (-S),
                               time (-t), version (-v), extension (-X)
      --time=WORD            with -l, show time as WORD instead of default
                               modification time: atime or access or use (-u);
                               ctime or status (-c); also use specified time
                               as sort key if --sort=time (newest first)
      --time-style=TIME_STYLE  time/date format with -l; see TIME_STYLE below
  -t                         sort by modification time, newest first
                             將文件依建立时间之先後次序列出
  -T, --tabsize=COLS         assume tab stops at each COLS instead of 8
                             假設制表符在每個COLS處停止，而不是8
  -u                         with -lt: sort by, and show, access time;
                             排序，顯示，訪問時間
                               with -l: show access time and sort by name;
                               使用-l:顯示訪問時間並按名稱排序
                               otherwise: sort by access time, newest first
                                否则:按访问时间排序，最新优先  
  -U                         do not sort; list entries in directory order
                            不排序;按目录顺序列出条目
  -v                         natural sort of (version) numbers within text
                             文本中的(版本)數字的自然排序
  -w, --width=COLS           set output width to COLS.  0 means no limit
                             將輸出寬度設置為COLS。0表示沒有限制
  -x                         list entries by lines instead of by columns
                             按行而不是按列列出条目
  -X                         sort alphabetically by entry extension
                             按條目擴展名按字母顺序排序
  -Z, --context              print any security context of each file
                             打印每個文件的任何安全上下文
  -1                         list one file per line.  Avoid '\n' with -q or -b
                             每行列出一个文件。避免使用-q或-b的'\n'
      --help     display this help and exit
                 顯示此帮助並退出
      --version  output version information and exit
                 輸出版本信息並退出。

The SIZE argument is an integer and optional unit (example: 10K is 10*1024).
Units are K,M,G,T,P,E,Z,Y (powers of 1024) or KB,MB,... (powers of 1000).
SIZE参数是一个整数和可选单元(例如:10K是10*1024)。单位是K,M,G,T,P,E,Z,Y(1024的幂)或KB,MB，…(1000的)。

The TIME_STYLE argument can be full-iso, long-iso, iso, locale, or +FORMAT.
FORMAT is interpreted like in date(1).  If FORMAT is FORMAT1<newline>FORMAT2,
then FORMAT1 applies to non-recent files and FORMAT2 to recent files.
TIME_STYLE prefixed with 'posix-' takes effect only outside the POSIX locale.
Also the TIME_STYLE environment variable sets the default style to use.

Using color to distinguish file types is disabled both by default and
with --color=never.  With --color=auto, ls emits color codes only when
standard output is connected to a terminal.  The LS_COLORS environment
variable can change the settings.  Use the dircolors command to set it.

Exit status:
 0  if OK,
 1  if minor problems (e.g., cannot access subdirectory),
 2  if serious trouble (e.g., cannot access command-line argument).

GNU coreutils online help: <https://www.gnu.org/software/coreutils/>
Full documentation at: <https://www.gnu.org/software/coreutils/ls>
or available locally via: info '(coreutils) ls invocation'

```
