#
```
Markdown文件
https://markdown.tw/
```
# 
```
Network Types: LAN, WAN, PAN, CAN, MAN, SAN, WLAN
https://www.youtube.com/watch?v=4_zSIXb7tLQ
```
```
Network Topologies (Star, Bus, Ring, Mesh, Ad hoc, Infrastructure, & Wireless Mesh Topology)
https://www.youtube.com/watch?v=zbqrNg4C98U
```

```
What is a DMZ? (Demilitarized Zone)
https://www.youtube.com/watch?v=dqlzQXo1wqo
```
```
NAT Explained - Network Address Translation
https://www.youtube.com/watch?v=FTUV0t6JaDA
```
# 網路硬體

```
Layer-1:repeater(1-1), hub(1-N)
Layer-2:bridgr, switch
Layer-3: router,L3-Switch
Layer-4: L4 switch
Layer-7: L7 switch, proxy
```



# 網路協定:

### OSI MODEL
```
OSI Model Explained | OSI Animation | Open System Interconnection Model | OSI 7 layers | TechTerms
https://www.youtube.com/watch?v=vv4y_uOneC0

7	應用層
application layer	例如HTTP、SMTP、SNMP、FTP、Telnet、SIP、SSH、NFS、RTSP、XMPP、Whois、ENRP、TLS
6	表現層
presentation layer	例如XDR、ASN.1、SMB、AFP、NCP
5	會議層
session layer	例如ASAP、ISO 8327 / CCITT X.225、RPC、NetBIOS、ASP、IGMP、Winsock、BSD sockets
4	傳輸層
transport layer	例如TCP、UDP、RTP、SCTP、SPX、ATP、IL
3	網路層
network layer	例如IP、ICMP、IPX、BGP、OSPF、RIP、IGRP、EIGRP、ARP、RARP、X.25
2	資料連結層
data link layer	例如乙太網路、權杖環、HDLC、影格中繼、ISDN、ATM、IEEE 802.11、FDDI、PPP
1	實體層
physical layer	例如線路、無線電、光纖
```
### TCP/IP MODEL
```

4	應用層
application layer	例如HTTP、FTP、DNS
（如BGP和RIP這樣的路由協定，儘管由於各種各樣的原因它們分別執行在TCP和UDP上，仍然可以將它們看作網路層的一部分）
3	傳輸層
transport layer	例如TCP、UDP、RTP、SCTP
（如OSPF這樣的路由協定，儘管執行在IP上也可以看作是網路層的一部分）
2	網路互連層
internet layer	對於TCP/IP來說這是網際網路協定（IP）
（如ICMP和IGMP這樣的必須協定儘管執行在IP上，也仍然可以看作是網路互連層的一部分；ARP不執行在IP上）
1	網路存取(連結)層
Network Access(link) layer	例如乙太網路、Wi-Fi、MPLS等。

```

### TCP/IP
```
傳輸控制協定（英語：Transmission Control Protocol，縮寫：TCP）是一種連接導向的、可靠的、基於位元組流的傳輸層通信協定，由IETF的RFC 793定義。在簡化的電腦網路OSI模型中，它完成第四層傳輸層所指定的功能。

網際協定（英語：Internet Protocol，縮寫：IP；也稱網際網路協定）是用於封包交換資料網路的一種協定。
```

### IEEE 802
```
https://zh.wikipedia.org/wiki/IEEE_802
```
```
IEEE 802中定義的服務和協定限定在OSI模型的最低兩層（即實體層和資料鏈路層）。

IEEE 802將OSI的資料鏈路層分為兩個子層:

Layer-2: 資料鏈路層===>  邏輯鏈路控制（LLC, Logical Link Control）
                媒介存取控制（MAC, Media Access Control）
Layer-1: 實體層
```
```
IEEE 802.1：高層區域網路協定（Bridging (networking) and Network Management）
IEEE 802.2：邏輯鏈路控制（Logical link control）

區域網路用的協定:
[超級重要]IEEE 802.3：乙太網路（Ethernet）
乙太網路實作了網路上無線電系統多個節點傳送資訊的想法，每個節點必須取得電纜或者通道才能傳送資訊，有時也叫作以太（Ether）。（這個名字來源於19世紀的物理學家假設的電磁輻射媒體-光以太。後來的研究證明光以太不存在。） 每一個節點有全球唯一的48位元位址也就是製造商分配給網卡的MAC位址，以保證乙太網路上所有節點能互相鑑別。由於乙太網路十分普遍，許多製造商把乙太網路卡直接整合進電腦主機板。

IEEE 802.4：權杖匯流排（Token bus）
IEEE 802.5：權杖環（Token-Ring）


IEEE 802.6：城域網（MAN, Metropolitan Area Network）
IEEE 802.7：寬頻TAG（Broadband LAN using Coaxial Cable）
IEEE 802.8：光纖分散式資料介面（FDDI）
IEEE 802.9：綜合業務區域網路（Integrated Services LAN）
IEEE 802.10：區域網路網路安全（Interoperable LAN Security）
[超級重要]IEEE 802.11：無線區域網路（Wireless LAN & Mesh）
IEEE 802.12：需求優先級（Demand priority）
IEEE 802.13：（未使用）
IEEE 802.14：電纜數據機（Cable modems）
IEEE 802.15：無線個人區域網路（Wireless PAN）
   IEEE 802.15.1：無線個人區域網路絡（WPAN, Wireless Personal Area Network）
   IEEE 802.15.4：低速無線個人區域網路絡（LR-WPAN, Low Rate Wireless Personal Area Network）
IEEE 802.16：寬頻無線接入（Broadband Wireless Access）
IEEE 802.17：彈性封包環傳輸技術（Resilient packet ring）
IEEE 802.18：無線電管制技術（Radio Regulatory TAG）
IEEE 802.19：共存標籤（Coexistence TAG）
IEEE 802.20：移動寬頻無線接入（Mobile Broadband Wireless Access）
IEEE 802.21：媒介獨立換手（Media Independent Handover）
IEEE 802.22：無線區域網（Wireless Regional Area Network）
IEEE 802.23：緊急服務工作群組（Emergency Services Working Group），2010年3月新發布
```
### ARP
```
Address Resolution Protocol (ARP) - Explained with example | Computer network | TechTerms
https://www.youtube.com/watch?v=EC1slXCT3bg

MAC Address
```
### ICMP
```
Internet Control Message Protocol
```
#### ICMP Message Format封包格式:

![ICMP 封包格式](icmp_header.gif)
```
ICMP 封包格式，其各欄位功能如下：
● 訊息型態（Message Type）：表示該 ICMP 所欲控制之訊息型態，共有 13 種型態，訊息型態之型態代表值如表 5-2 所示。
● 編碼（Code）：對各種訊息型態進一步說明工作內容。
● 檢查集檢查碼（Checksum）：對該封包檢查集錯誤偵測。
● 訊息說明（Message description）：依照不同的控制訊息，而有不同的說明方式。
```
#### Message Type
```
    ICMP 訊息功能

[重要]0  Echo Reply（回應答覆）
[重要]3  Destination Unreachable（目的地無法到達）

4 Source Quench（來源抑制）

[重要]5 Redirect（改變傳輸路徑）

[重要]8 Echo Request（回應要求）

9 Router Advertisement（路由器宣傳）
10 Router Solicitation（路由器懇請）
11 Time Exceeded for a Datagram（溢時傳輸）
12 Parameter Problem on a Datagram（參數問題）
13 Timestamp Request（時間標籤要求）
14 Timestamp Reply（時間標籤回覆）
15 Information Request（資訊要求）（停用）
16 Information Reply（資訊回覆）（停用）
17 Address Mask Request（位址遮罩要求）
18 Address Mask Reply（位址遮罩回覆）
```
### ICMP 封裝

![ICMP 封裝](icmp_encap.gif)

### ICMP 常用指令
```
ping 
tracert| Traceroute
如何使用 TRACERT 疑難排解 Windows 中的 TCP/IP 問題
https://support.microsoft.com/zh-tw/help/314868/how-to-use-tracert-to-troubleshoot-tcp-ip-problems-in-windows
```
```
tracert www.pchome.com.tw

在上限 30 個躍點上 Tracing route to 11.1.0.1 over a maximum of 30 hops
追蹤 www.pchome.com.tw [210.59.230.39] 的路由:

  1    <1 ms    <1 ms    <1 ms  172.20.155.254
  2    10 ms     5 ms     6 ms  172.16.190.253
  3    <1 ms    13 ms     1 ms  120-114-151-14.ksu.edu.tw [120.114.151.14]
  4     *        *        *     要求等候逾時。
  5     *        *        *     要求等候逾時。
  6     *        *        *     要求等候逾時。
  7     *        *        *     要求等候逾時。
```
### TCP vs UDP 
```
TCP vs UDP Comparison
https://www.youtube.com/watch?v=uwoD5YsGACg

傳輸控制協定（英語：Transmission Control Protocol，縮寫：TCP）是一種連接導向的、可靠的、基於位元組流的傳輸層通信協定，由IETF的RFC 793定義。在簡化的電腦網路OSI模型中，它完成第四層傳輸層(Layer-4 Transport)所指定的功能。

用戶資料報協定（UDP）是同一層(Layer-4 Transport)內另一個重要的傳輸協定。
```


### SSL, TLS, HTTP, HTTPS 
```
SSL, TLS, HTTP, HTTPS Explained
https://www.youtube.com/watch?v=hExRDVZHhig
```

###  Proxy Server
```
What is a Proxy Server?
https://www.youtube.com/watch?v=5cPIukqXe5w
```

### FTP (File Transfer Protocol), SFTP, TFTP Explained.
```
FTP (File Transfer Protocol), SFTP, TFTP Explained.
https://www.youtube.com/watch?v=tOj8MSEIbfA
```

### DNS
```

```

### DNS
```

```

### DNS
```

```
