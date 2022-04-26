

#define _CRT_SECURE_NO_WARNINGS
#include <stdlib.h>
#include <stdio.h>


void main()
{
	int num1=6;
	int* P1;
	P1 = &num1;  //P1 takes the address memory from num1;
	*P1 = 10;
	printf("%d \n", *P1);
	printf("%d", num1);

}

====================================




#define _CRT_SECURE_NO_WARNINGS
#include <stdlib.h>
#include <stdio.h>


void swap(int* P1, int* P2) //p1 gets num1's adress and p2 gets num2's adresss
{
	int temp;
	temp = *P1; //The star means u want to get the value of the address.
	*P2 = *P1;
	*P1 = temp;

}


void main()
{
	int num1 = 10, num2 = 5;
	swap(&num1, &num2); //it gives the address of num 1 and 2
	printf("%d %d\n", num1, num2);
}
