```
import java.util.Scanner; //匯入Scanner類別庫
public class DoMath {//類別D開始

	public static void main(String[]args) {//主函式開始
		sumof2number();//呼叫副函式計算2數的和
		sumof3number();
		sumof4number();
		sumof5number();
		in2number();//呼叫副函式輸入並計算2數的和
		in3number();
	}//主函式結束
	
	public static void sumof2number() {//副函式 計算2數的和開始
	int num1,num2,sum;
	num1=10;//指定整數10給變數num1
	num2=20;//指定整數20給變數num2
	sum=num1+num2;//指定10+20的結果給變數sum
	System.out.printf("總和=%d\n",sum);
	}//副函式結束
	
	public static void sumof3number() {//副函式 計算3數的和開始
		int num1=10,num2=20,num3=30,sum;
		sum=num1+num2+num3;
		System.out.printf("3個數字%d+%d+%d的和=%d\n",num1,num2,num3,sum);
		//"\%d"代表 輸出格式為十進位的(decimal)
	}//副函式結束
	
	public static void sumof4number() {//副函式計算4數的和開始
		int num1=10,num2=20,num3=30,num4=40,sum;
		sum=num1+num2+num3+num4;
		System.out.printf("%d+%d+%d+%d=%d\n",num1,num2,num3,num4,sum );
	}//副函式結束
	
	public static void sumof5number() {//副函式計算5數的和開始
		int num1=10,num2=20,num3=30;
		int num4=40,num5=50,sum;sum=num1+num2+num3+num4+num5;
		System.out.printf("%d+%d+%d+%d+%d=%d\n",
				  num1,num2,num3,num4,num5,sum);
	
	}//副函式結束
	
	public static void in2number() {//副函式輸入2數並計算2數的和開始
		Scanner sc=new Scanner(System.in);
		System.out.printf("請輸入數字1:");
		int num1=sc.nextInt();//建立物件sc,使user能輸入整數
		System.out.printf("請輸入數字2:");
		int num2=sc.nextInt();
		int sum=num1+num2;
		System.out.printf("%d+%d=%d\n",num1,num2,sum);
	}//副函式結束
	
	public static void in3number() {//副函式輸入3數並計算3數的和開始
		Scanner sc=new Scanner(System.in);
		System.out.printf("請輸入數字1:");
		int num1=sc.nextInt();
		System.out.printf("請輸入數字2:");
		int num2=sc.nextInt();
		System.out.printf("請輸入數字3:");
		int num3=sc.nextInt();
		int sum=num1+num2+num3;
		System.out.printf("%d+%d+%d=%d\n",num1,num2,num3,sum);
	}//副函式結束
}//類別結束
```

# 程式結果
```
總和=30
3個數字10+20+30的和=60
10+20+30+40=100
10+20+30+40+50=150
請輸入數字1:100
請輸入數字2:200
100+200=300
請輸入數字1:11
請輸入數字2:22
請輸入數字3:33
11+22+33=66

```
