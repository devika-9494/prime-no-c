# prime-no-c
4 in 1 brush for nails
https://github.com/devika-9494/tom-and-jerry/blob/main/lcm.md
https://github.com/devika-9494/array/commit/9cad7c64d752cf0cbc6f4939e3135a35d42c24e7
https://github.com/devika-9494/timeandminute
https://github.com/devika-9494/matrix
https://github.com/devika-9494/employee
https://github.com/devika-9494/switch-case/blob/main/switchcase.md
#include <stdio.h>
 
int primeno(int, int);
 
int main()
{
    int num, check;
    printf("Enter a number: ");
    scanf("%d", &num);
    check = primeno(num, num / 2);
    if (check == 1)
    {
        printf("%d is a prime number\n", num);
    }
    else
    {
        printf("%d is not a prime number\n", num);
    }
    return 0;
}
 
int primeno(int num, int i)
{
    if (i == 1)
    {
        return 1;
    }
    else
    {
       if (num % i == 0)
       {
         return 0;
       }
       else
       {
            return primeno(num, i - 1);
       }       
     }
   }
      
       
       
