# fibonacci_number
I wrote Fibonacci numbers with a recursive function.


#include <stdlib.h>
#include <stdio.h>

int fibonacci(int number)
{
	if(number == 0)
		return 0;
	else if(number == 1)
		return 1;
	else
		return fibonacci(number - 1) + fibonacci(number - 2);
}

int main()
{
	int number;
	printf("enter a number:");
	scanf("%d",&number);
	
	if(number < 0)
		printf("negatif sayı girmeyiniz!!!");
	else
		printf("%d.fibonacci number: %d",number,fibonacci(number));
	
	return 0;
}
