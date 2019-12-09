```
import java.util.Scanner; //匯入Scanner類別庫
public class DoMath {//類別開始

	public static void main(String[]args) {//主函式開始
		sumof2number();//呼叫副函式
		sumof3number();
		sumof4number();
		sumof5number();
		in2number();
		in3number();
	}//主函式結束
	
	public static void sumof2number() {//副函式開始
	int num1,num2,sum;
	num1=10;
	num2=20;
	sum=num1+num2;
	System.out.printf("總和=%d\n",sum);
	}//副函式結束
	
	public static void sumof3number() {//副函式開始
		int num1=10,num2=20,num3=30,sum;
		sum=num1+num2+num3;
		System.out.printf("3個數字%d+%d+%d的和=%d\n",num1,num2,num3,sum);
	}//副函式結束
	
	public static void sumof4number() {
		int num1=10,num2=20,num3=30,num4=40,sum;
		sum=num1+num2+num3+num4;
		System.out.printf("%d+%d+%d+%d=%d\n",num1,num2,num3,num4,sum );
	}
	public static void sumof5number() {
		int num1=10,num2=20,num3=30;
		int num4=40,num5=50,sum;sum=num1+num2+num3+num4+num5;
		System.out.printf("%d+%d+%d+%d+%d=%d\n",
				          num1,num2,num3,num4,num5,sum);
	
	}
	public static void in2number() {
		Scanner sc=new Scanner(System.in);
		System.out.printf("請輸入數字1:");
		int num1=sc.nextInt();
		System.out.printf("請輸入數字2:");
		int num2=sc.nextInt();
		int sum=num1+num2;
		System.out.printf("%d+%d=%d\n",num1,num2,sum);
	}
	public static void in3number() {
		Scanner sc=new Scanner(System.in);
		System.out.printf("請輸入數字1:");
		int num1=sc.nextInt();
		System.out.printf("請輸入數字2:");
		int num2=sc.nextInt();
		System.out.printf("請輸入數字3:");
		int num3=sc.nextInt();
		int sum=num1+num2+num3;
		System.out.printf("%d+%d+%d=%d\n",num1,num2,num3,sum);

	}
}
```
