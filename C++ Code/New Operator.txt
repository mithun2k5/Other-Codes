//Program-1-New and delete Operator

#include<iostream>
#include<string>

using namespace std;

int main()
{
int *p=new int(5);//it returns address value
*p=1;
cout<<*p<<"\n"<<p<<endl;
delete p;
cout<<*p<<"\n"<<p<<endl;
system("pause");
return 0;
}

//Program-2-New and delete Operator

#include<iostream>

using namespace std;

class person
{
public:
	int age;
	char name;
};
///////////////////////////////0///
int main()
{
person *p=new person;
(*p).age=30;
cout<<(*p).age<<endl;
p->age=40;
cout<<p->age<<endl;
system("pause");
return 0;
}
///////////////////////////////