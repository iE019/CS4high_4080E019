# top 用於實時顯示process 的動態

```

top --help
top: inappropriate '-help'
Usage:
  top -hv | -bcEHiOSs1 -d secs -n max -u|U user -p pid(s) -o field -w [cols]
root@kali:~# top -help
  procps-ng 3.3.15
Usage:
  top -hv | -bcEHiOSs1 -d secs -n max -u|U user -p pid(s) -o field -w [cols]

d : 改變顯示的更新速度，或是在交談式指令列( interactive command)按 s
q : 沒有任何延遲的顯示速度，如果使用者是有superuser 的權限，則top 將會以最高的優先序執行
c : 切換顯示模式，共有兩種模式，一是只顯示執行檔的名稱，另一種是顯示完整的路徑與名稱S : 累積模式，會將己完成或消失的子行程( dead child process ) 的CPU time 累積起來
s : 安全模式，將交談式指令取消, 避免潛在的危機
i : 不顯示任何閒置(idle) 或無用(zombie) 的行程
n : 更新的次數，完成後將會退出top
b : 批次檔模式，搭配"n" 參數一起使用，可以用來將top 的結果輸出到檔案內

```
