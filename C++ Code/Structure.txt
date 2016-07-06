#include<iostream>
#include<string>
#include<sstream>

using namespace std;

struct student
{
string name;
int grade;
};

int main()
{
student pupil1;
student pupil2;
cout<<"Enter student name::";
getline(cin,pupil1.name);
cout<<"Enter student grade::";
cin>>pupil1.grade;
cout<<"Enter student name::";
cin>>pupil2.name;
cout<<"Enter student grade::";
cin>>pupil2.grade;
cout<<"Name"<<"               "<<"Grade"<<endl;
cout<<pupil1.name<<"                 "<<pupil1.grade<<endl;
cout<<pupil2.name<<"                 "<<pupil2.grade<<endl;

system("pause");
return 0;
}
