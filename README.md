import java.util.Scanner;
public class Main{
    public static void main(String[]args){
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int sum=0,rem=0,temp=n;
        int digits=String.valueOf(n).length();
        while(temp!=0)
        {
            rem=temp%10;
            sum+=Math.pow(rem,digits);
            temp/=10;
        }
        if(sum==n)
        {
            System.out.println("armstrong");
        }
        else
        {
            System.out.println("not an armstrong");
        }
    }
}# armstrong-number
