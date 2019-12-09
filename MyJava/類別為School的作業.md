```
public class School {//類別學校開始
	private String About_kunshan;//宣告私有的全域變數 關於崑山
	private String Academic_institution;//宣告私有的全域變數 教學單位
	private String Administrative_unit;//宣告私有的全域變數 行政單位
public School() {}//預設建構子
public School(String A_k,String A_i,String A_u) {//自定義建構子開始
	this.About_kunshan=A_k;//指定字串參數A_k給全域變數About_kunshan
	this.Academic_institution=A_i;//指定字串參數A_i給全域變數Academic_institution
	this.Administrative_unit=A_u;//指定字串參數A_u給全域變數Administrative_unit
}//自定義建構子結束

public void setAbout_kunshan(String A_k) {//副函式設定關於崑山開始
	this.About_kunshan=A_k;//指定字串參數A_k給全域變數About_kunshan
}//副函式設定關於崑山結束

public void setAcademic_institution(String A_i) {//副函式設定教學單位開始
	this.Academic_institution=A_i;//指定字串參數A_i給全域變數Academic_institution
}//副函式設定教學單位結束

public void setAdministrative_unit(String A_u) {//副函式設定行政單位開始
	this.Administrative_unit=A_u;//指定字串參數A_u給全域變數Administrative_unit
}//副函式設定行政單位結束
	
public String getAbout_kunshan() {//副函式得到關於崑山開始
	return About_kunshan;//回傳字串關於崑山
}//副函式得到關於崑山結束

public String getAcademic_institution() {//副函式得到教學單位開始
	return Academic_institution;//回傳字串教學單位
}//副函式得到教學單位結束

public String getAdministrative_unit() {//副函式得到行政單位開始
	return Administrative_unit;//回傳字串行政單位
}//副函式得到行政單位結束

public void printSchoolInfo() {//副函式列印出學校資訊開始
	System.out.println("關於崑山:"+About_kunshan+"\t"
			+"教學單位:"+Academic_institution+"\t"
			+"行政單位:"+Administrative_unit);//列印出字串，並彼此之間運用跳脫字元\t間隔4格
}//副函式列印出學校資訊結束

public static void main(String[]args) {//主函式開始
	School obj_s1=new School("學校校史","電子工程系","教務處");//建立物件obj_s1,並指定字串參數給全域變數
	obj_s1.printSchoolInfo();//列印出關於崑山:學校校史    教學單位:電子工程系    行政單位:教務處
	obj_s1.setAcademic_institution("資訊工程系");//更改學校obj_s1的教學單位
	obj_s1.printSchoolInfo();//列印出關於崑山:學校校史    教學單位:資訊工程系    行政單位:教務處
	System.out.println(obj_s1.getAbout_kunshan());//直接列印出關於崑山內的字串,並換行
	School obj_s2=new School("校內地圖","環境工程系","學生事務處");//建立物件obj_s2,並指定字串參數給全域變數
	obj_s2.printSchoolInfo();//列印出關於崑山:校內地圖    教學單位:環境工程系    行政單位:學生事務處
	School obj_s3=new School();//建立物件obj_s3(無參數)
	obj_s3.printSchoolInfo();//列印出關於崑山:null    教學單位:null    行政單位:null
}//主函式結束

}//類別學校結束
```

# 程式結果
```
關於崑山:學校校史	教學單位:電子工程系	行政單位:教務處
關於崑山:學校校史	教學單位:資訊工程系	行政單位:教務處
學校校史
關於崑山:校內地圖	教學單位:環境工程系	行政單位:學生事務處
關於崑山:null	教學單位:null	行政單位:null
```
