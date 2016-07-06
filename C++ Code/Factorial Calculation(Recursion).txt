//Recursion is to call a funtion within itsellf for repetitive use considering base value::

#include<iostream>

using namespace std;

int factorial(int x);

int main()
{
int n;
cout<<"Enter number::";
cin>>n;
cout<<"The factorial of number is::"<<factorial(n)<<endl;
system("pause");
return 0;
}


int factorial(int x)
{
if (x==1)//this is the base condition
{
return 1;
}
else 
{
return x*factorial(x-1);
}
}


