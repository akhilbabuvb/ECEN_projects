#include<stdio.h>
#include<string.h>
#define zeros 0
#define char_space 32
#define one 1
#define ten 10
#define str_size 20
#define size 500
#define size2 100

int main()
{
int i,count=zeros,cap,pen,car=zeros,temp=zeros,lander;

char sun[str_size]="will    you  call me",

moon[size],star[size],num[size2],store=zeros,eyes=zeros;

for(i=zeros;i<ten;i++)
{
  num[i]=zeros;
}
i=zeros;

 while(sun[i]!=zeros)
 {
 car++;
 moon[i]=sun[i];
 i++;
 }
if(sun[i]==zeros)
{
moon[i]=zeros;
}
i=zeros;
for(i=zeros;moon[i]!=zeros;i++)
{
if(moon[i]==char_space)
{
count++;
if(count>one)
{
for(pen=i;pen!=car;pen++)
{
moon[pen]=moon[pen+one];
}
count=count-one;
i=i-one;
store++;
}
}
if(moon[i]!=char_space)
{
 count=zeros;
if(store!=zeros)
{
num[eyes]=store;
eyes++;
store=zeros;
}
}
}
cap=i;
strcpy(star,moon);
i=zeros;
eyes=zeros;
car=cap;
while(moon[i]!=zeros)
{

if(moon[i]==char_space)
{
  if(num[eyes]==zeros){
    break;}
if(num[eyes]!=zeros){
   lander=(i+temp);
for(pen=zeros;pen<num[eyes];pen++)
{
for(cap;cap>=lander;cap--)
{
star[cap+one]=star[cap];
}
car++;
cap=car;
}
}
temp=temp+num[eyes];
eyes++;
}
i++;
}
printf("%s\n",sun);
printf("%s\n",moon);
printf("%s\n",star);
}


