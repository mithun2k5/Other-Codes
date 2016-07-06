//Print Number

#include<iostream>

using namespace std;

class bakir
{
int n;
public:
	void getdata(void);
    void display(void);
};

void bakir::getdata(void)
{
cout<<"Enter number of n::";
cin>>n;
}

void bakir::display(void)
{
	cout<<"\nThe numbers are:";
	if (n>0)
	{
	for(int i=0;i<=n;i++)
	{	
	cout<<"\n"<<i;
	}
	}
	else 
	{
	for(int i=0;i>=n;i--)
	{	
	cout<<"\n"<<i;
	}	
	}
}


int main()
{
bakir m;
m.getdata();
m.display();
system("pause");
return 0;
}

//Program-2 Print Number

#include<iostream>

using namespace std;

int main()
{
int n,x;
cout<<"Give input::";
cin>>n;
cout<<"The triangle will be::"<<endl;
for(int i=1;i<=n;i++)
{
for(int j=1;j<=i;j++)
{
	cout<<"        1 ";
}
cout<<endl;
}
system("pause");
system("pause");
return 0;
}

//Print triangle

#include<iostream>

using namespace std;

int main()
{
int n=0;
cout<<"Give input::";
cin>>n;
for (int i=1;i<=n;i++)
{
for(int j=1;j<=n-i;j++)
{
cout<<" ";
}
for (int k=1;k<=i*2-1;k++)
{
cout<<"*";
}
cout<<endl;
cout<<endl;
}
system ("pause");
system("pause");
return 0;
}



