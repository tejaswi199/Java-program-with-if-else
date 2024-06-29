import java.util.Scanner;
public class main{
    public static void main(String [] args){
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter amount:");
        int a=sc.nextInt();
        if(a<=500){
            System.out.println("No discount;Amount paid is "+a);
        }
        else if(a>500 && a<=1000){
            System.out.println("10% discount provided");
            double d=a*0.1;
            System.out.println("Amount paid after discount is " + (a-d));
        }
        else if(a>=1001 && a<=2000){
            System.out.println("20% discount provided");
            double d=a*0.2;
            System.out.println("Amount paid after discount is " + (a-d));
        }
        else if(a>=2001 && a<=5000){
            System.out.println("30% discount provided");
            double d=a*0.3;
            System.out.println("Amount paid after discount is " + (a-d));
        }
        
        else{
            System.out.println("No discount ;Amount paid is "+a);
        }
    }
}
