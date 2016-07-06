//Program-1

#include<iostream>

using namespace std;

int main()
{
char age;
cout<<"Enter the letter associated with your age:\n"
	"Press\n"
	"(A) if your age 17 or below\n"
	"(B) if your age 18 to 65\n"
	"(C) if your age 65 above\n";
cin>>age;
cout<<"\nYour ticket price will be::";

switch(age)
{
case 'a':
case 'A':cout<<"10 dollar";
break;
case 'b':
case 'B':cout<<"15 dollar";
break;
case 'c':
case 'C':cout<<"20 dollar";
break;
default: cout<<"Invalid entry";
break;
}
cout<<endl; 
system ("pause");
return 0;
}

//Program-2

#include<iostream>
#include<string>

using namespace std;

int option;

class operation
{
private:
	int a,b;
public:
	void getdata();
	void addition();
	void subtraction();
	void division();
	void multiplication();
};

void operation::getdata()
{
cout<<"Enter 1st number::";
cin>>a;
cout<<"\nEnter 2nd number::";
cin>>b;
cout<<"\nEnter option::"
	"\nEnter 1 for addition"
	"\nEnter 2 for subtraction"
	"\nEnter 3 for division"
	"\nEnter 4 for multiplication"
	"\nEnter 5 for quit"<<endl;
cin>>option;
}

void operation::addition()
{
cout<<"The addition is::"<<a+b<<endl;
}

void operation::subtraction()
{
	cout<<"The subtraction is::"<<a-b<<endl;
}

void operation::multiplication()
{
	cout<<"The multiplication is::"<<a*b<<endl;
}

void operation::division()
{
	cout<<"The division is::"<<a/b<<endl;
}


int main()
{
operation p;
p.getdata();
while(option!=5)
{
switch(option)
{
case 1:
	p.addition();
	break;
case 2:
	p.subtraction();
	break;
case 3:
	p.division();
	break;
case 4:
	p.multiplication();
	break;
default:
	cout<<"Please enter appropriate number."<<endl;
	break;
}
cout<<"\nEnter option::"
	"\nEnter 1 for addition"
	"\nEnter 2 for subtraction"
	"\nEnter 3 for division"
	"\nEnter 4 for multiplication"
	"\nEnter 5 for quit"<<endl;
cin>>option;
}
system("pause");
return 0;
}

