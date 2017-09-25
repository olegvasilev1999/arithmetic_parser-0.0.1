# arithmetic_parser-0.0.1




#include "stdafx.h" 
#include "iostream"

using namespace std;

int main() {

	char oper ;
	int a, b;

	cin >> a >> oper;
	if (oper == '<' || oper == '>') {
		cin >> oper >> b;
	}
	else {
		cin >> b;
	}


	switch (oper) {
	case '+': cout << (int)(a + b) << endl; break;
	case '-': cout << (int)(a - b) << endl; break;
	case '*': cout << (int)(a * b) << endl; break;
	case '/': cout << (double)(a / b) << endl; break;
	case '%': cout << (int)(a % b) << endl; break;
	case '&': cout << (int)(a % b) << endl; break;
	case '|': cout << (int)(a | b) << endl; break;
	case '^': cout << (int)(a ^ b) << endl; break;
	case '>': cout << (int)(a >> b) << endl; break;
	case '<': cout << (int)(a << b) << endl; break;
	}

	system("pause");
	cin.get();

	return 0;
}
