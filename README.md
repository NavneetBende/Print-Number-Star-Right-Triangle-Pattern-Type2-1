PRINT PATTERN  7*8*9*10 4*5*6
For any input number N Print the following code – For below code N=4

7*8*9*10
4*5*6
2*3
1
PREREQUISITE:
Basic knowledge in Java programming, usage of loops.

ALGORITHM:
Take input from user i.e number of lines required (N value).
Take two loops one for each line (say ‘i’) and other for each digit in a particular line (say ‘j’). i starts from N and j starts from 1.
Take a result variable (say ‘a’) and initialize it with (i*(i-1))/2+1.
Here ‘i’ loop is used to access each line from n to 1 and ‘j’ loop is used to print values in each line. j loop is executed until it reaches i value.
Print ‘a’ value along with * and post increment  until the j loop reaches a value less than i.
Print the final value ‘a’ of each line and go to next line.
Repeat the ‘i’ loop until it reaches 1.
CODE IN JAVA:
import java.lang.*;
import java.io.*;
class Main
{
    public static void main (String[]args) throws IOException
    {
        BufferedReader br =new BufferedReader (new InputStreamReader (System.in));
        int n, i, j, a = 0;
        System.out.print ("Enter the N value:");
        n = Integer.parseInt (br.readLine ());
    
        for (i = n; i >= 1; i--)
        {
	        a = (i * (i - 1)) / 2 + 1;
	        for (j = 1; j < i; j++)
	        {
	            System.out.print ((a++) + "*");
	        }
	        System.out.println (a++);
        }
    }
}
 

TAKING INPUT:


DISPLAYING OUTPUT:
