
#include<stdio.h>
#include<string.h>
int main ()
{
	char str[100];
	gets(str);
	int i,upper=0,lower=0,digit=0;
	for(i=0;str[i]!='\0';i++)
	{
		if(isupper(str[i])) 
		{
			upper=upper+1;
		}
		else if(islower(str[i]))
		{
			lower=lower+1;
		}
		else if(isdigit(str[i]))
		{
			digit=digit+1;
		}
	}
	printf("count of uppercase characters=%d\n",upper);
	printf("count of lowercase characters=%d\n",lower);
	printf("count of numbers=%d\n",digit);
	return 0;
}
