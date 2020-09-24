#不使用%和/，判断一个整数是否能被3整除
#3是一个比较特殊的数，任何一个整数和3相乘就等于这个整数与它左移一位后的数相加，所以上述算法就是利用这个特性，第一步通过&取出最后一位，因为左移一位后的末尾是0，所以通过将这个整数右一位得到是原数字的#末尾，依此类推


include<stdio.h>
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
