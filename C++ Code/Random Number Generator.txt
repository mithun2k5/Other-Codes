#include<iostream>
#include<ctime>
#include<cstdlib>

using namespace std;

int main()
{
int max,random_number;
cout<<"Enter maximum number::";
cin>>max;
srand(time(0));
random_number= (rand()%max)+1;
cout<<"The random number is::"<<random_number<<endl;
system("pause");
return 0;
}
