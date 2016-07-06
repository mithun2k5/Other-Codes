//Program-1-Recursion

#include<iostream>
#include<string>
using namespace std;

void returnword(string x,string y);

int main()
{
string text,word,mithun;
cout<<"Enter string::";
getline(cin,text);
cout<<"Enter word::";
getline(cin,word);
returnword(text,word);
system("pause");
return 0;
}

void returnword(string x,string y)
{
int location;
location=x.find(y);
if (location!=string::npos)
{
cout<<"TRUE"<<endl;
}
else
{ 
cout<<"FALSE"<<endl;
}
}


/*#include<iostream>
#include <stdio.h>
#include <string>
#include<sstream>

using namespace std;

int main ()
{
  char str[] ="This is a simple string";
  char *pch;
  pch = strstr (str,"simple");
  //strncpy (pch,"sample",6);
  //puts (str);
  cout<<pch<<endl;
  system("pause");
  return 0;
}*/

//Recursive Addition

#include<iostream>
#include<sstream>

using namespace std;

int add(int n);

int main()
{
int n;
cout<<"Give integer value::";
cin>>n;
cout<<"The summation of digit is::";
cout<<add(n)<<endl;
system("pause");
return 0;
}

int add(int n)
{
int a,b;
if (n<10)
return n;
else 
{ 
a=(n/10);
b=(n%10);
return (add(a)+add(b));
}
}



