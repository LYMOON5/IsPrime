#include<stdio.h>
#include<math.h>
#include<string.h>

//写一个判断素数的函数
bool IsPrime(int n)
{
	int i;
	for(i=2;i<=sqrt((float)n);i++)
	{
		if(n%i==0)
			return false;
	}
	return true;
}

int main()
{
	int n;                 
	scanf("%d",&n);
	if(IsPrime(n))
		printf("%d是素数\n",n);
	else
		printf("%d不是素数\n",n);
    
	return 0;
}
