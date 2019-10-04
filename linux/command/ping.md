# ping 用於檢測主機

```

ping --help
ping: invalid option -- '-'
Usage: ping [-aAbBdDfhLnOqrRUvV64] [-c count] [-i interval] [-I interface]
            [-m mark] [-M pmtudisc_option] [-l preload] [-p pattern] [-Q tos]
            [-s packetsize] [-S sndbuf] [-t ttl] [-T timestamp_option]
            [-w deadline] [-W timeout] [hop1 ...] destination
Usage: ping -6 [-aAbBdDfhLnOqrRUvV] [-c count] [-i interval] [-I interface]
             [-l preload] [-m mark] [-M pmtudisc_option]
             [-N nodeinfo_option] [-p pattern] [-Q tclass] [-s packetsize]
             [-S sndbuf] [-t ttl] [-T timestamp_option] [-w deadline]
             [-W timeout] destination

-d使用套接字的SO_DEBUG功能。
-c <完成次數>設置完成要求響應的次數。
-f極限檢測。
-i <間隔秒數>指定收發信息的間隔時間。
-I <網絡界面>使用指定的網絡接口送出數據包。
-l <初步加載>設置在送出要求信息之前，先行發出的數據包。
-n只輸出數值。
-p <範本樣式>設置填滿數據包的範本樣式。
-q不顯示指令執行過程，開頭和結尾的相關信息除外。
-r忽略普通的路由表，直接將數據包直接插入主機上。
-R記錄路由過程。
-s <數據包大小>設置數據包的大小。
-t <存活數值>設置存活數值TTL的大小。
-v詳細顯示指令的執行過程。


```
