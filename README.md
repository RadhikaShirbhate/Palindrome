# Palindrome
public class Palindrome
{

	public static void main(String[] args)
 {
		int n = Integer.parseInt(args[0]);
		
		if(n<0)
			System.out.println("The given number is -ve kindly provide the +ve number only");
		else if(n<99)
			System.out.println("This program can check the operation for the 3 number only");
		
		else if(n<999 && n>99)
		{
		int r,sum=0,temp;
		temp=n;
		while(n>0)
		{
			r=n%10;
			sum=(sum*10)+r;
			n=n/10;
		}	
		if(temp==sum)
			System.out.println("The number is pallindrome");
		else
			System.out.println("The number is not pallindrome");}
}

}
