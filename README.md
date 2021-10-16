# Binary-System
//sum and multiplication in binary

#include <stdio.h>

int show(int n)
{
    int a[10];
    int i=0;
 
   while(n != 0)
   {
       a[i]=n%2;
       n=n/2;
       i++;
   }
   for(i=i-1;i>=0;i--)
   printf("%d",a[i]);
    return 0;
}

int main()
{
   int n1,n2,sum,product;
   printf("Enter two numbers");
   scanf("%d %d",&n1,&n2);
   sum = n1+n2;
   product = n1*n2;
   printf("In arabic system,sum=%d",sum);
   printf("\nIn binary system,sum=");
   show(sum);
   printf("\n\n In arabic system,product=%d",product);
   printf("\nIn binary system,product=");
   show(product);
   
}

