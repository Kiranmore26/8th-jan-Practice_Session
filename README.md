package Anudip;

import java.util.Scanner;

/*
WAP to accept choice from user and accordingly display the output
1:Given no is even or odd
2:Find out the grade (accept marks of 5 subject)
3:Accept no and find out cube if no is divisble by 5
4:Accept 3 nofrom user and find out the greatest
*/
public class Practice {

	public static void main(String[] args) 
	{
		int Choice;
		Scanner sc = new Scanner(System.in);
		System.out.println("Enter Your Choice:  ");
		Choice=sc.nextInt();
		switch (Choice) 
		{
		case 1:
			System.out.println("Given no is even or odd");
				int num;
				System.out.println("Enter the number:");
				num=sc.nextInt();
					if(num%2==0)
					{
						System.out.println("The no is even");
					}
					else
					{
						System.out.println("The no is odd");
					}
					
			break;
		
		case 2:
			System.out.println("Find out the grade (accept marks of 5 subject)");
			int Total_marks=500;
			int English;
			int Hindi;
			int marathi;
			int maths;
			int Science;
			System.out.println("Enter the marks of English:");
			English=sc.nextInt();
			System.out.println("Enter the marks of Hindi:");
			Hindi=sc.nextInt();
			System.out.println("Enter the marks of Marathi:");
			marathi=sc.nextInt();
			System.out.println("Enter the marks of maths:");
			maths=sc.nextInt();
			System.out.println("Enter the marks of Science:");
			Science=sc.nextInt();
			 int Total_obtainmarks=English+marathi+maths+Hindi+Science;
			 System.out.println("Total obtain marks are "+Total_obtainmarks);
			 int percentage = (maths+marathi+Hindi+English+marathi/500)*100;
				
				if(percentage>=80)
				{
					System.out.println("A+ Grade");
				}
				else if(percentage>=60)
				{
					System.out.println("A Grade");
				}
				else
				{
					System.out.println("B Grade");
				}
				
			

		
			
			break;
			
		case 3:
			  System.out.println("Accept no and find out cube if no is divisble by 5");
			  int a;
			  System.out.println("Enter A no");
			  a=sc.nextInt();
			  if(a%5==0)
			  {
				  System.out.println("No is divisble by 5 ");
				  int cube=a*a*a;
				  System.out.println("Cube of that no is :  "+ cube);
			  }
			  else
			  {
				  System.out.println("THe no is not Divisble by 5");
			  }
			break;
			
		case 4:
			System.out.println("Accept 3 nofrom user and find out the greatest");
			int no1,no2,no3;
			System.out.println("Enter 1st no:");
			no1=sc.nextInt();
			System.out.println("Enter 2nd no:");
			no2=sc.nextInt();
			System.out.println("Enter 3rd no:");
			no3=sc.nextInt();
			
			if(no1>no2 && no1> no3)
			{
				System.out.println("Number 1 is greater" +no1);
			}
			else if(no2>no1 && no2> no3)
			{
				System.out.println("Number 2 is greater" +no2);

			}
			else if(no3>no1 && no3> no2)
			{
				System.out.println("Number 3 is greater" +no3);

			}
			
			break;

		default:
			System.out.println("Invalid Choice");
			break;
		}

	}

}
