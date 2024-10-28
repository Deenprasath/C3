rev string using loop

#include <stdio.h>
#include<string.h>
int main()
{
   
   char str[100], temp;
   int i,left,right,len;
   printf("\n enter the string");
   scanf("%s",str);
   len = strlen(str);
   left=0;
   right= len-1;
   for(i=left;i<right;i++)
   {
       temp = str[i];
       str[i]=str[right];
       str[right]=temp;
       right--;
       
   }
   printf("\n after reverse %s", str);
   return 0;
}
