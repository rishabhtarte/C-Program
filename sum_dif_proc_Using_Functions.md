
//Sum_dif_product Using Functions

#include<conio.h>
#include<stdio.h>
#include<math.h>
float f=0;
float s=0;
float ans=0;

int main()
{
while(1)
{		
float sum();
float dif();
float pro();
int a=0;

printf("Enter First value\n");
scanf("%f",&f);
printf("Enter Second value\n");
scanf("%f",&s);
printf("Enter Operation to Perform\n");
printf("\n1: Addition \n2: Absolute Substraction \n3: Product \n0: Exit \n");
scanf("%d",&a);


if(a==1){
	ans=sum();
	}
if(a==2){
	ans=dif();
}
if(a==3){
	ans=pro();
}

printf("The Result is= %.2f \n",ans);
if(a==0){
	printf("\n BYE");
	break ;

}
}

return 0;

}


float sum()
{
	float sum=0;
	sum=(f+s);
	return sum;
}
float dif()
{
	float dif=0;
	dif=f-s;
	dif=fabs(dif);
	return dif;
}
float pro()
{
	float pro=0;
	pro=f*s;
	return pro;
}
