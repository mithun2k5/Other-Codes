#include <iostream>
#include <sstream>

using namespace std;

int main()
{
int number=0,count=0;
cout<<"Enter number:";
cin >> number;
for (int a=1;a<=number;a++)
{
if (number%a==0)
{
count ++;
}
}
if (count==2)
{
cout <<"\nIt is a Prime number";
}
else
{
cout << "\nIt is not a prime number";
}
system("pause");
return 0;
}