#include<iostream>

using namespace std;

void printarray(int thearray[],int size);

int main()
{
int arrays[3]={10,20,30,};
printarray(arrays,3);
system("pause");
return 0;
}

void printarray(int thearray[],int size)
{
cout<<"The array elements are::"<<endl;
for (int i=0;i<size;i++)
{
cout<<thearray[i]<<endl;
}
}