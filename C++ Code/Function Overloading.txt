#include<iostream>
#include<string>

using namespace std;

void addition(int a,int b)
{
int c;
c=a+b;
cout <<"The int addition is::"<<c<<endl;
}

void addition(float e,float f)
{
float d;
d=e+f;
cout<<"The float addition is::"<<d<<endl;
}

int main()
{
//int a=2,b=2;
float e=2.5,f=2.5;
addition(2,2);
addition(e,f);
system("pause");
return 0;
}