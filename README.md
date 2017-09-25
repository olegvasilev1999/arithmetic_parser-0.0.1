# arithmetic_parser-0.0.1



#include "stdafx.h"
#include "iostream"

using namespace std;

int main()
{

	char oper;
	int a, b ;

	cout << "put your  \n";
	cin >> a >> oper >> b;

	switch (oper) {
	case '+': cout << "result:" << (int)a + (int)b <<endl; break;
	case '-': cout << "result:" << (int)a - b << endl; break;
	case '*': cout << "result:" << (int)a * b << endl; break;
	case '/': cout << "result:" << (double)a / b << endl; break;
	case '%': cout << "result:" << (int)a % b << endl; break;
	case '&': cout << "result:" << (int)a % b << endl; break;
	case '|': cout << "result:" << (int)(a | b) << endl; break;
	case '^': cout << "result:" << (int)(a ^ b) << endl; break;
	case '>': cout << "result:" << (int)(a >> b) << endl; break;
	case '<': cout << "result:" << (int)(a << b) << endl; break;
	}

	system("pause");
	cin.get();
	
	return 0;
	

}
