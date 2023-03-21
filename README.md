# Unit-Converter-In-C-Language-
A unit converter is a computer program that allows users to convert measurements from one unit of measurement to another. The program can be designed to convert measurements for various types of units, such as length, temperature, and more.

#include <stdio.h>
float calculate(int a){
int input1,input2,value;
switch (a){

case 1:
printf("enter the meter ");
scanf("%d",&input1);
value = input1 /1000;
printf("the value in km is %d",value);
break;

case 2:
printf("enter the meter ");
scanf("%d",&input1);
value = input1 * 39.37;
printf("the value in inches is %d",value);
break;

case 3:
printf("enter the meter ");
scanf("%d",&input1);
value = input1 * 3.281;
printf("the value in feet is %d",value);
break;

case 4:
printf("enter the seconds ");
scanf("%d",&input1);
value = input1 / 60;
printf("the value in minutes is %d",value);
break;

case 5:
printf("enter the second ");
scanf("%d",&input1);
value = input1 / 3600;
printf("the value in hours is %d",value);
break;

case 6:
printf("enter the joules ");
scanf("%d",&input1);
value = input1 / 4184;
printf("the value in kilocalories is %d",value);
break;

case 7:
printf("enter the temperature in centigrate ");
scanf("%d",&input1);
value = (input1*1.8) + 32;
printf("the value in farhenhite is %d",value);
break;

case 8:
printf("enter your speed in km/h:");
scanf("%d",&input1);
printf("enter your distance in km:");
scanf("%d",&input2);
value = input2/input1;
printf("the time required to reach your destination is %d
",value);
printf("hours");

case 9:
printf("enter your time in h:");
scanf("%d",&input1);
printf("enter your distance in km:");
scanf("%d",&input2);
value = input2/input1;
printf("the required to reach your destination on time is %d
",value);
printf("km/h");
}
}

int main() {
int choice;
printf("Unit Conversion \n");

printf("to convert m into km enter 1 \n");

printf("to convert m into inches enter 2 \n");

printf("to convert m into feet enter 3 \n");

printf("to convert seconds into minute enter 4 \n");
printf("to convert second into hours enter 5 \n");

printf("to convert joules into calories enter 6 \n");

printf("to convert centigrades into farhenhite enter 7 \n");

printf("enter the speed and distance to calculate how much time is required to reach at your destination enter 8 \n");

printf("enter the time and distance to calculate how much speed
 is required enter 9 \n");
 
printf("Enter your Choice :");

scanf("%d",&choice);

calculate(choice);
return 0;
}
