# arithmetic_parser-0.0.1




#include "stdafx.h" 
#include "iostream"

using namespace std;

int main() {

	char oper,op ;
	int a, b;

	cin >> a >> oper;

	if (oper == '<' || oper == '>') {
		cin >> op >> b;
		if ( oper == '<' && op == '<' ) {
		 cout << (int)(a << b) << endl; 	
		}
		else if (oper == '>' && op == '>') {
			cout << (int)(a >> b) << endl;
		}
		else cout << "ERROR";
	
	}
		else {
			cin >> b;
			
			switch (oper) {
		case '+': cout << (int)(a + b) << endl; break;
		case '-': cout << (int)(a - b) << endl; break;
		case '*': cout << (int)(a * b) << endl; break;
		case '/': cout << (double)(a / b) << endl; break;
		case '%': cout << (int)(a % b) << endl; break;
		case '&': cout << (int)(a % b) << endl; break;
		case '|': cout << (int)(a | b) << endl; break;
		case '^': cout << (int)(a ^ b) << endl; break;
			default: cout << "ERROR";
		}
		}

	system("pause");
	cin.get();

	return 0;
}
