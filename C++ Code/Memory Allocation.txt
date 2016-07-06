//Dynamic memory allocation///4 functions are there
#include<iostream>
#include<string>

using namespace std;

int main()
{
//malloc funciton
int *p;
p= (int *)malloc(sizeof(int));
*p=10;
cout<<"Malloc::"<<p<<"\n"<<*p<<endl;
//realloc funciton
p=(int*)realloc(p,sizeof(int));
cout<<"Realloc::"<<p<<"\n"<<*p<<endl;

//calloc function
int *q;
q=(int*)calloc(1,1000);
*q=1;
cout<<"Calloc::"<<q<<"\n"<<*q<<endl;
///free function
free(q);
system("pause");
return 0;
}
