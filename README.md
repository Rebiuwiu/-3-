#include<stdio.h>
int main(){
	int n;
	int s;
	scanf("%d",&n);
	while(n>0)
	{
		s = n&1;
		n>>=1;
		n = n-s;
		
	}
	if(n == 0)
	{
		printf("yes");
	}
	else
	{
		printf("no");
	}
}
