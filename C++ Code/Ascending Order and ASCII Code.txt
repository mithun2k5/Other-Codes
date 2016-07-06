//Ascending

#include<iostream>

using namespace std;

int main()
{
int a[100],n,b,flag,c,mitun;
cout<<"Enter number of elements in the array::"<<endl;
cin>>n;
cout<<"The elements are::\n";
for(int i=0;i<=n-1;i++)
{
cin>>a[i];
}
cout<<"The ascending order of number is::"<<endl;
flag=1;
while(flag)
{
flag=0;
for (int i=1;i<=n-1;i++)
{
if (a[i-1]>a[i])
{
b=a[i-1];
a[i-1]=a[i];
a[i]=b;
flag=1;
}
}
}
for (int i=0;i<=n-1;i++)
{
cout<<a[i]<<endl;
}
system("pause");
return 0;
}

///Sorting name alphabetically
///Unable to use strcmp() function also


#include<string>
#include<iostream>
#include<string>


using namespace std;

int main()
{
int n;
string name[100],initialName[100],temp=0,a,b;
cout<<"Give number of names to be sorted::";
cin>>n;
cout<<"The names are::";
for (int i=0;i<=n-1;i++)
{
	getline(cin,name[i]);
	initialName[i]=name[i];
}
for (int i=0;i<=n-1;i++)
{
for (int j=i+1;j<n;j++)
{
	if(name[i]>name[j])
	{
	temp=name[i];
	name[i]=name[j];
	name[j]=temp;
	}
}
}
cout<<"Given Name            Sorted name::";

for (int i=0;i<=n-1;i++)
{
	cout<<initialName[i]<<"         "<<name[i]<<endl;
}
system("pause");
return 0;
}

//Finding ASCII Code

#include <iostream>
#include<string>

using namespace std;

int main()
{
int n;
cout<<"Text to ASCII converter"<<endl<<"Enter text to convert into ASCII - ";
string text;   //defining input type, which is single character
int ascii;   //defining that ASCII code will be numeric integer
getline(cin,text);   //taking input from user
n=text.length();
for (int i=0;i<=n-1;i++)
{
ascii = static_cast<int>(text[i]);//converting the input character into ASCII code
cout<<endl<<"ASCII code is "<<ascii<<"\n"<<endl; //displaying the ASCII code
}
system("pause");
return 0;
} 