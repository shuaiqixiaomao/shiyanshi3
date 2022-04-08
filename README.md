计算器0
#include <stdio.h>
#include <string.h>

int main()
{
	char a[]="3+4";

	int left=a[0]-'0';
	int right=a[2]-'0';
    int result=left+right;

	printf("result=%d\n",result);
	return 0;
}
计算器1
#include <stdio.h>
#include <string.h>

int main()
{
	char jia[]="1+2+2+1+2+5+4-1-3+4-8";
	int result=jia[0]-'0';

	for(int i=0;i<100;i++)
	{
		if(jia[i]=='+')
		{
			result=result+(jia[i+1]-'0');
		}
		else if(jia[i]=='-')
		{
			result=result-(jia[i+1]-'0');
		}
	}
	printf("%d\n",result);
	return 0;}
计算器2
#include <stdio.h>
#include <string.h>

int main()
{ 
	char chen[]="2*2/4*1/1*2*3/2";
    int result=chen[0]-'0';

	for(int i=0;i<100;i++)
	{
		if(chen[i]=='*')
		{
			result=result*(chen[i+1]-'0');
		}
		
		else if(chen[i]=='/')
		{
			result=result/(chen[i+1]-'0');
		}
	}
	
	
	printf("%d\n",result);
	return 0;}
