
public class Student {//類別學生開始
	private String name;//宣告私有的全域變數 姓名
	private String id;//宣告私有的全域變數 學號
	private String major;//宣告私有的全域變數 科系(主修)

public Student() {}//預設建構子
public Student(String n,String i,String m) {//自定義建構子開始
	this.name=n;//指定字串參數n給全域變數name
	this.id=i;//指定字串參數i給全域變數id
	this.major=m;//指定字串參數m給全域變數major
}//自定義建構子結束

public void setName(String n) {//副函式設定姓名開始
	this.name=n;//指定字串參數n給全域變數name
}

public void setId(String i) {//副函式設定學號開始
	this.id=i;//指定字串參數i給全域變數id
}

public void setMajor(String m) {//副函式設定科系開始
	this.major=m;//指定字串參數m給全域變數major
}

public String getName() {//副函式得到姓名開始
	return name;//回傳全域變數name的字串
}//副函式得到姓名結束

public String getId() {//副函式得到學號開始
	return id;//回傳全域變數id的字串
}//副函式得到學號結束

public String getMajor() {//副函式得到科系開始
	return major;//回傳全域變數major的字串
}//副函式得到科系結束

public void printStudentInfo() {//副函式列印出學生資訊開始
	System.out.println("學生姓名:"+name+"\t"
			+"學號:"+id+"\t"
			+"科系:"+major);//列印出字串，並彼此之間運用跳脫字元\t間隔4格
}//副函式列印出學生資訊結束

public static void main(String[]args) {//主函式開始
	Student obj_s1=new Student("金厲害","4080E000","資工系");//建立物件obj_s1,並指定字串參數給全域變數
	obj_s1.printStudentInfo();//列印出學生姓名:金厲害	學號:4080E000	科系:資工系
	obj_s1.setId("4080E001");//更改學生obj_s1的學號
	obj_s1.printStudentInfo();//列印出學生姓名:金厲害	學號:4080E001	科系:資工系
	System.out.println(obj_s1.getName());//列印出金厲害
	Student obj_s2=new Student("曾漂亮","4080F001","時尚系");//建立物件obj_s2,並指定字串參數給全域變數
	obj_s2.printStudentInfo();//列印出學生姓名:曾漂亮	學號:4080F001	科系:時尚系
	Student obj_s3=new Student();//建立物件obj_s3(無參數)
	obj_s3.printStudentInfo();//列印出學生姓名:null	學號:null	科系:null
}//主函式結束

}//類別Student結束
