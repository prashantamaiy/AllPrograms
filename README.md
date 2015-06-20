//This program will retur the frequency of each work.
public class HelloWorld {

	public static void main(String[] args) 
	{
		String str = "Prashant awan sameer awan sameer viju";
		String arry[] = str.split(" ");

		for(int i = 0; i < arry.length; i ++)
		{
			int count = 1;
			for(int j = i+1;j < arry.length; j++)
			{

				int n = arry[i].compareToIgnoreCase(arry[j]);

				if(n == 0)
				{
					count++;

					arry[j] = "";

				}

			}
			if(arry[i] != "")
			{
				System.out.println(arry[i]+ " " +count);
			}


		}

	}

}

