Find maximum and minimum element (Using one dimensional array)
Aim
Given different prices of a vegetable which is varying through the day (from morning to evening) Write a C program to find out the best buy price and sell price for the maximum profit (using one dimensional array).
Program
#include <stdio.h>
int main()
{
int n, a[10], min, max, count=0, i;
printf("Enter the total no. of elements: \n");
scanf("%d", &n);
printf("Enter the elements : \n");
for (i=0; i<n; i++)
{
scanf("%d", &a[i]);
}
min = max = a[0];
for (i=1; i<n; i++)
{
if (a[i] < min)
{
min = a[i];
}
if (a[i]> max)
{
max = a[i];
}
}
}
printf("Minimum number: %d\n", min); 
printf("Maximum number: %d\n", max); return 0;

Weights of 10 students of your class who are standing in a line is given in a random order. Write a C program to find out the heavy person whose weight is the sum of previous two persons.
Program
#include<stdio.h>
int main()
{
int n, a[10], i, t=0;
printf("Enter the no. of students standing in the line: "); scanf("%d", &n);
printf("Enter thier Weights: \n");
for(i=0; i<n; i++)
f
scanf("%d",&a[i]);
}
for(i=2; i<n; i++)
{
if(a[i]== a[i-2]+a[i-1])
{
printf("\n Yes...Weight element at position %d is sum of previous two positions (Weights)...", i);
t=1;
}
}
if(t==0)
printf("\n No more Weight element found to be the sum of previous two positions (Weights)...");
return 0;
