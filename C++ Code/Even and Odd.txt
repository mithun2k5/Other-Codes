//Even and Odd
#include <iostream>
#include <string>
#include <sstream>

using namespace std;

int main()
{
    int number=0;
	cout << "Enter the number to check it either even or not:";
	cin >> number;
	if(number%2==0)
	{
	cout << "\n\n" << number << ":" << "is even";
	}
	else
	{
	cout << "\n\n" << number << ":" << "is odd";
	}
	system("pause");

	return 0; 
}