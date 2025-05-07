# Calculator
A simple calculator (+-*/)
#include <iostream>
using namespace std;

int main()
{
	char operation, choice = 'Y';
	int operand1, operand2, answer;
	while (choice == 'Y')
	{
		cout << "Enter the expression you would like to solve: " << endl;
		cin >> operand1 >> operation >> operand2;

		switch (operation)
		{
		case '+':
			answer = operand1 + operand2;
			cout << "The answer is: " << answer << endl;
			break;
		case '-':
			answer = operand1 - operand2;
			cout << "The answer is: " << answer << endl;
			break;
		case '*':
			answer = operand1 * operand2;
			cout << "The answer is: " << answer << endl;
			break;
		case '/':
			answer = operand1 / operand2;
			cout << "The answer is: " << answer << endl;
			break;
		default:
			cout << "Please enter a valid operation" << endl;
		}
		cout << "Would you like to continue using the calculator (Y/N)?" << endl;
		cin >> choice;
		choice = toupper(choice);
	}
	cout << "Goodbye" << endl;
	return 0;
}
