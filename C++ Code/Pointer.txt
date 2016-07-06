//Pointer is a special variable which stores the memory address of the variable.


#include<iostream>

using namespace std;

int main()
{
int fish=5;
int *fishpointer;
fishpointer=&fish;
cout<<fishpointer<<endl;
system("pause");
return 0;
}

//*=Content of operator
//&=Address of operator


#include<iostream>
#include<string>


using namespace std;

int main()
{
int *p;
int x;
x=25;
p=&x;
cout<<p<<endl;
system ("pause");
return 0;
}

//3rd Program-Pointer

#include<iostream>

using namespace std;
void passByValue(int x);
void passByReference(int *x);

int main()
{
int x=15;
int y=40;
passByValue(x);
passByReference(&y);
cout<<x<<endl;
cout<<y<<endl;
system("pause");
return 0;
}


void passByValue(int x)
{
	x=15;
}

void passByReference(int *x)
{
*x=55;
}

//4th Program-Pointer

#include<iostream>
#include<string>

using namespace std;

int main()
{
int a[100],n;
int *p;
p=a;
for (int i=0;i<=3;i++)
{
cin>>a[i];
}
for (int i=0;i<=3;i++)
{
cout<<*(p+i)<<endl;
}

system("pause");
return 0;
}

//Program-5 on pointer

#include<iostream>
#include<sstream>
#include<string>

using namespace std;

int main()
{
int firstvalue,secondvalue;
int *mypointer;
mypointer=&firstvalue;
*mypointer=10;
cout<<firstvalue<<"\n";
cout<<mypointer;
system ("pause");
return 0;
}