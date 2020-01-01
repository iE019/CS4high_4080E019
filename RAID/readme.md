# 容錯式磁碟陣列（Redundant Array of Independent Disks，RAID）
```
  容錯式磁碟陣列（Redundant Array of Independent Disks，RAID），簡稱磁碟陣列。
  利用虛擬化儲存技術把多個硬碟整合起來，成為一個或多個硬碟陣列組。
  目的為提升效能或資料冗餘(重複)，或是兩者同時提升。
  普通用戶主要是應用在需要大容量儲存空間的工作，例：視訊及音訊製作。
    
  RAID 0也稱為帶區集。它將兩個以上的Disks(磁碟)並聯起來，
  成為一個大容量的Disk。
  在存放Data時，分段後分散儲存在這些Disks中，因為讀寫時都可以並列處理，
  所以在所有的級別中，RAID 0的速度是最快的。
  但是RAID 0沒有冗餘功能及容錯能力，
  如果一個Disk遭到物理損壞，All Data(全部資料)都會消失。
  
  RAID 1是兩組以上的多個Disks相互作鏡像，
  在一些多執行緒作業系統中能有很好的讀取速度。
  只要一個Disk正常即可維持運作，可靠性最高。
  其原理為在Main Hard Disk(主硬碟)上存放Data的同時也在鏡像硬碟上寫一樣
  的Data，
  當Main Hard Disk遭到物理損壞時，鏡像硬碟則代替Main Hard Disk的工作。
  因為有鏡像硬碟做Data back up(資料備份)，
  所以RAID 1的資料安全性在所有的RAID級別上來說是最好的。
  但無論用多少Disks做RAID 1，僅算一個Disk的容量，
  所以是所有RAID中，Disk利用率最低的一個級別。
  
  RAID 0+1是先鏡像再將Data到分割兩組Hard Disk。
  它將所有的硬碟分為兩組，每組各自構成為RAID 0作為最低組合，
  而將兩組硬碟組合為RAID 1運作。
  只要有一個硬碟受損，同組RAID 0的所有硬碟都會停止運作，
  只剩下其他組的硬碟運作，可靠性較低。
```
