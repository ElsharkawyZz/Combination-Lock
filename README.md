# Combination-Lock

using System;
					
public class Program
{
	public static void Main()
	{
				int size=int.Parse(Console.ReadLine());

		string pass1=Console.ReadLine();
		string pass2=Console.ReadLine();
		int path1;
		int path2;
		int count=0;
		for(int i=0;i<size;i++)
		{
			int num1=pass1[i]-'0';
			int num2=pass2[i]-'0';
			
			if(num1<=6)
			{
				path1=Math.Abs(num1-num2);
			path2=Math.Abs(num1-0)+Math.Abs(10-num2);
				if(path1>path2||path1==path2)
			{
			Console.WriteLine(path2);
					count+=path2;
					Console.WriteLine(" step 1 ___");
			}else
			{
				Console.WriteLine(path1);
					count+=path1;
					Console.WriteLine(" step 2 ___");
			}

			
			}else 
			{
				path1=Math.Abs(num1-num2);
			path2=Math.Abs(num1-10)+Math.Abs(num2);
				if(path1>path2||path1==path2)
			{
			Console.WriteLine(path2);
					count+=path2;
					Console.WriteLine(" step 3 ___");
			}else
			{
				Console.WriteLine(path1);
					count+=path1;
					Console.WriteLine(" step 4 ___");
			}
			
			}
			
			
		 
		}
		Console.WriteLine(" count ___");
			Console.WriteLine(count);
	}
}
