#include<iostream>
#include<sstream>
#include<math.h>

using namespace std;

int fibonacchi(int n);

int main()
{
int n;
cout<<"Enter number of elements:"<<endl;
cin>>n;
cout<<"The fibonacchi series is::"<<endl;
cout<<fibonacchi(n)<<endl;
system("pause");
return 0;
}

int fibonacchi(int n)
{
	if (n==0)
	{
	return 0;
	}
	else if (n==1)
	{
	return 1;
	}
	else
		return fibonacchi(n-1)+fibonacchi(n-2);
}
