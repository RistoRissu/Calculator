import java.util.Scanner;
public class Calculator
{
	public static double q=0, table[]=new double[3];
	public static void main(String[] args)
	{
		Scanner program = new Scanner(System.in);
		q=0;
		while (q==0)
		{
			double x=0;
			System.out.println("CALCULATOR");
			System.out.println("stempinski.p@gmail.com");
			System.out.println();
			System.out.println("1. Addition");
			System.out.println("2. Subtraction");
			System.out.println("3. Multiplication");
			System.out.println("4. Division");
			x = program.nextDouble();
			if (x==1){dodawanie();}
			else if (x==2){odejmowanie();}
			else if (x==3){mnozenie();}
			else if (x==4){dzielenie();}
		}
	}

	public static double dodawanie()
	{
		System.out.println("Result: "+table[1]);
		Scanner dodawanie = new Scanner(System.in);
		System.out.println("Addition");
		System.out.println();
		q=1;
		while (q==1)
		{
			if (table[1]==0)
			{
				System.out.print("Fist number: ");
				table[1] = dodawanie.nextDouble();
			}
			System.out.print("Next number: ");
			table[2] = dodawanie.nextDouble();
			double c=table[1]+table[2];
			System.out.println("Result: "+c);
			System.out.print("Continue? [Y=1  N<>1]: ");
			q=dodawanie.nextDouble();
			table[1]=c;
		}   
		q=0;
		return table[1];
	}

	public static double odejmowanie()
	{
		System.out.println("Result: "+table[1]);
		Scanner dodawanie = new Scanner(System.in);
		System.out.println("Subtraction");
		System.out.println();
		q=1;
		while (q==1)
		{
			if (table[1]==0)
			{
				System.out.print("First number: ");
				table[1] = dodawanie.nextDouble();
			}
			System.out.print("Next number: ");
			table[2] = dodawanie.nextDouble();
			double c=table[1]-table[2];
			System.out.println("Result: "+c);
			System.out.print("Continue? [Y=1  N<>1]: ");
			q=dodawanie.nextDouble();
			table[1]=c;   	
		}
		q=0;
		return table[1];
	}

	public static double mnozenie()
	{
		System.out.println("Result: "+table[1]);
		Scanner dodawanie = new Scanner(System.in);
		System.out.println("Multiplication");
		System.out.println();
		q=1;
		while (q==1)
		{
			if (table[1]==0)
			{
				System.out.print("First number: ");
				table[1] = dodawanie.nextDouble();
			}
			System.out.print("Next number: ");
			table[2] = dodawanie.nextDouble();
			double c=table[1]*table[2];
			System.out.println("Result: "+c);
			System.out.print("Continue? [Y=1  N<>1]: ");
			q=dodawanie.nextDouble();
			table[1]=c;
		}
		q=0;
		return table[1];
	}

	public static double dzielenie()
	{
		System.out.println("Result: "+table[1]);
		Scanner dodawanie = new Scanner(System.in);
		System.out.println("Division");
		System.out.println();
		q=1;
		while (q==1)
		{
			if (table[1]==0)
			{
				System.out.print("First number: ");
				table[1] = dodawanie.nextDouble();
			}
			System.out.print("Next number: ");
			table[2] = dodawanie.nextDouble();
			double c=table[1]/table[2];
			System.out.println("Result: "+c);
			System.out.print("Continue? [Y=1  N<>1]: ");
			q=dodawanie.nextDouble();
			table[1]=c;
		}
		q=0;
		return table[1];
	}
}