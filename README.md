import java.util.Scanner;
public class Series4
{
    int n;
    double ans=0;
    void input()
    {
        Scanner sc= new Scanner(System.in);
        System.out.println("Enter the number of terms");
        n= sc.nextInt();
    }
    
    void answer()
    {
        double sum =1,pro=1;
        for(int i=2;i<=n;i++)
        {
            sum= sum+i;
            pro = pro*i;
            ans = ans+ (sum/pro);
            
        }
        System.out.println("The sum of the series is: " + ans);
    }
    
    public static void main()
    {
        Series4 obj=new Series4();
        obj.input();
        obj.answer();
        
    }
}
