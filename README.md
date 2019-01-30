# product-of-first-largest-and-second-largest
#include<stdio.h>
#include<stdlib.h>
int main()
{
int n,a[1000],r,i,j,max1,max2;
scanf("%d",&n);
for(i=0;i<n;i++)
{
r=n%10;
a[i]=r;
n=n/10;
}
max1=a[0];
max2=a[0];
for(j=0;j<i;j++)
{
if(a[j]>max1)
{
max1=a[j];
}
}
for(j=0;j<i;j++)
{
if(a[j]<max2&&a[j]>max1)
{
max2=a[j];
}
}
printf("%d",max1*max2);
}
