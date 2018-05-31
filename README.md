# school
package assignmenttwo;
import java.util.Scanner;
public class question3
{
    public static void main(String[] args)
    { 
        Scanner keyboard = new Scanner(System.in);
        double income, incomeTax=0;
        
        System.out.print("Enter Income: $ ");
         income = keyboard.nextDouble();
         String answer;
         
        while (income != -1)
        {
         if (income==0)
         {
             System.out.println("Invalid Income");
         }
         else if (income > 0 && income <20000)
         { 
             incomeTax = 0;
             System.out.printf("Income Tax is : $ %.2f \n" ,incomeTax);
             System.out.print("Enter Income again, [Enter -1 to quit]: $ ");
             income = keyboard.nextDouble();
         }
         else if (income >= 20000 && income < 30000)
         {
             incomeTax = (income - 20000) * 0.02;
             System.out.printf("Income Tax is : $ %.2f \n" ,incomeTax);
             System.out.print("Enter Income again, [Enter -1 to quit]: $ ");
             income = keyboard.nextDouble();
         }
         else if (income >= 30000 && income < 40000)
         {
             incomeTax = (income - 30000) * 0.035 + 200;
             System.out.printf("Income Tax is : $ %.2f \n" ,incomeTax);
             System.out.print("Enter Income again, [Enter -1 to quit]: $ ");
             income = keyboard.nextDouble();
         }
         else if (income >= 40000 && income < 80000)
         {
             incomeTax = (income - 40000) * 0.07 + 550;
             System.out.printf("Income Tax is : $ %.2f \n" ,incomeTax);
             System.out.print("Enter Income again, [Enter -1 to quit]: $ ");
             income = keyboard.nextDouble();
         }
         else if (income >= 80000 && income < 120000)
         {
             incomeTax = (income - 80000) * 0.115 + 3350;
             System.out.printf("Income Tax is : $ %.2f \n" ,incomeTax);
             System.out.print("Enter Income again, [Enter -1 to quit]: $ ");
             income = keyboard.nextDouble();
         }
         else if (income >= 120000 && income < 160000)
         { 
             incomeTax = (income - 120000) * 0.15 + 7950;
             System.out.printf("Income Tax is : $ %.2f \n" ,incomeTax);
             System.out.print("Enter Income again, [Enter -1 to quit]: $ ");
             income = keyboard.nextDouble();
         }
         else if (income >= 160000 && income < 200000)
         {
             incomeTax = (income - 160000) * 0.17 + 13950;
             System.out.printf("Income Tax is : $ %.2f \n" ,incomeTax);
             System.out.print("Enter Income again, [Enter -1 to quit]: $ ");
             income = keyboard.nextDouble();
         }
         else if (income >= 200000 && income < 320000)
         {
             incomeTax = (income - 200000) * 0.18 + 20750;
             System.out.printf("Income Tax is : $ %.2f \n" ,incomeTax); 
             System.out.print("Enter Income again, [Enter -1 to quit]: $ ");
             income = keyboard.nextDouble();
         }
         else 
         {
             incomeTax = (income - 320000) * 0.20 + 42350;
             System.out.printf("Income Tax is : $ %.2f \n" ,incomeTax); 
             System.out.print("Enter Income again, [Enter -1 to quit]: $ ");
             income = keyboard.nextDouble();
         }
        
        } 
        System.out.println("----- END OF PROGRAM -----");     
    }
}

// Design a Java program to accept income from the user; compute the income tax to be paid and display the income and the tax payable on the screen. Your code should contain appropriate validations and must focus on code optimisation. Modify the code to repeat the program until the user enters an income value of -1. 
