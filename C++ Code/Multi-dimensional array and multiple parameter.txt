//Multidimensional array

#include<iostream>

using namespace std;


int main()
{
	int arrays[2][3]={{1,2,3},{4,5,6}};
for (int row=0;row<2;row++)
{
for(int column=0;column<3;column++)
{
cout<<arrays[row][column]<<"  ";

}
cout<<endl;
}
system("pause");
return 0;
}

//Multiple Parameters

#include<iostream>

using namespace std;

int addnumber(int x,int y)
{
int answer=x+y;
return answer;
}

int main()
{
cout<<addnumber(10,10)<<endl;
system ("pause");
return 0;
}