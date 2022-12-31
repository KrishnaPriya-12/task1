package task1.salary;
import java.util.Scanner;
public class TaxCalculator {
	public static void main(String xyz[])
	   {
		   
		    Scanner sc = new Scanner(System.in);
			System.out.print("Enter Basic Salary :- ");
			int salary = sc.nextInt();
			float taxRate = 0;
			double hra =1;
			double da = 1;
			hra = 0.15 * salary;
			da	= 0.6 * salary;
			
			if(salary<500000)
			{
				taxRate = 0;				
			}
			
			else if(salary>5000000 && salary<1000000)
			{
				taxRate = 20;	
			}
			
			else
			{
				taxRate = 30;
			}
				
			float tax = salary * taxRate/100;
			
			System.out.print("For Salary "+salary);
			System.out.println("HRA is"+ hra);
			System.out.println("DA is"+da);
			System.out.println("Tax is"+tax);
			
			
			
		}
		
	   

}

