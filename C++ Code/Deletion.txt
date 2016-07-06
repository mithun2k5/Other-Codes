//Deletion by element in the array

#include<iostream>
#include<string>

using namespace std;

int main()
{
int a[100],n,m,temp=0,pos,option;
cout<<"Enter the number of elements:";
cin>>n;
cout<<"Enter elements::"<<endl;
for (int i=0;i<=n-1;i++)
{
	cin>>a[i];
}
cout<<"The sorted elements are::"<<endl;
for (int i=0;i<=n-1;i++)
{
for (int j=i+1;j<=n-1;j++)
{
	if(a[i]>a[j])
	{
	temp=a[i];
	a[i]=a[j];
	a[j]=temp;
	}
}
}
for (int i=0;i<=n-1;i++)
{
	cout<<a[i]<<endl;
}
cout<<"Enter number to delete::";
cin>>m;
for (int i=0;i<=n-1;i++)
{
if(a[i]==m)
{
pos=i;
break;
}
}
for (int i=pos;i<=n-1;i++)
{
	a[i]=a[i+1];
}
cout<<"The newly formed array::"<<endl;
for (int i=0;i<=n-2;i++)
{
cout<<a[i]<<endl;
}
system("pause");
return 0;
}

//Delete by position

#include<iostream>
#include<string>

using namespace std;

int main()
{
int a[100],n,m,temp=0,pos,option;
cout<<"Enter the number of elements:";
cin>>n;
cout<<"Enter elements::"<<endl;
for (int i=0;i<=n-1;i++)
{
	cin>>a[i];
}
cout<<"The sorted elements are::"<<endl;
for (int i=0;i<=n-1;i++)
{
for (int j=i+1;j<=n-1;j++)
{
	if(a[i]>a[j])
	{
	temp=a[i];
	a[i]=a[j];
	a[j]=temp;
	}
}
}
for (int i=0;i<=n-1;i++)
{
	cout<<a[i]<<endl;
}
cout<<"Enter position to delete::";
cin>>m;
for (int i=0;i<=n-1;i++)
{
if(i==m-1)
{
pos=i;
break;
}
}
for (int i=pos;i<=n-1;i++)
{
	a[i]=a[i+1];
}
cout<<"The newly formed array::"<<endl;
for (int i=0;i<=n-2;i++)
{
cout<<a[i]<<endl;
}
system("pause");
return 0;
}