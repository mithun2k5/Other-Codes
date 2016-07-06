#include<iostream>
#include<string>

using namespace std;

class highest_value
{
private:
	int a[100],n,temp;
public:
	void getdata();
	void comparison();
};

void highest_value::getdata()
{
	cout<<"Enter the number of elements::";
	cin>>n;
	cout<<"\nEnter elements::";
	for (int i=0;i<=n-1;i++)
	{
	cin>>a[i];
	}
}

void highest_value::comparison()
{
	for (int i=0;i<=n-1;i++)
	{
	for (int j=i+1;j<=n-1;j++)
	{
	if (a[i]>a[j])
	{
	temp=a[i];
	a[i]=a[j];
	a[j]=temp;
	}
	}	
	}
cout<<"The highest number is::"<<a[n-1]<<endl;
}

int main()
{
highest_value p;
p.getdata();
p.comparison();
system("pause");
return 0;
}