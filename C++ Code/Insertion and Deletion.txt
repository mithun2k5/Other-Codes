//Insertion and deletion::

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
cout<<"Press::\n1 to insert element\n" 
	          "2 to delete elements by entering element\n" 
			  "3 to delete elements by position\n"
			  "4 to quit::";
cin>>option;

while(option!=4)
{
switch(option)
{
case 1:
cout<<"Enter the new element:"<<endl;
cin>>m;
for (int i=0;i<=n-1;i++)
{
	if(a[0]>=m) 
	{
	pos=i;
	break;
	}
	
else if (a[i]<=m && m<=a[i+1])
{
pos=i+1;
break;
}
else if (m>a[n-1])
{
pos=n;
break;
}
}
for (int i=n;i>pos;i--)
{
a[i]=a[i-1];
}
a[pos]=m;
cout<<"The newly formed sorted array::"<<endl;
for (int i=0;i<=n;i++)
{
	cout<<a[i]<<endl;
}
n=n+1;
break;
case 2:
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
cout<<"The newly formed sorted array::"<<endl;
for (int i=0;i<=n-2;i++)
{
cout<<a[i]<<endl;
}
n=n-1;
break;
case 3:
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
n=n-1;
break;
default:
	cout<<"\nYou have entered wrong option\n"<<endl;
}
cout<<"Press:: 1 to insert element\n" 
	          "2 to delete elements by entering element\n" 
			  "3 to delete elements by position\n"
			  "4 to quit::";
cin>>option;
}
system("pause");
return 0;
}
