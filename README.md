/* 
   SPOJ Problem Set
   Problem Code: ADD_REV
*/

#include <stdio.h>
#include <stdlib.h>

int main()
{
    int num1 , num2 , sum = 0 , rev1 = 0 , rev2 = 0;
    printf("Enter the first number:\n");
    scanf("%d",&num1);
    printf("Enter the second number:\n");
    scanf("%d",&num2);
    while(num1!=0)
    {
       rev1 = (num1%10)+(rev1*10);
       num1 = num1/10;
    }
    printf("Reverse is : %d\n",rev1);

    while(num2!=0)
    {
        rev2 = (num2%10)+(rev2*10);
        num2 = num2/10;
    }
    printf("Reverse is : %d\n",rev2);

    sum = rev1+rev2;
    printf("Sum of Reversed numbers is : %d",sum);

    return 0;
}
