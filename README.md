#include <iostream>
#include <cmath>
using namespace std;

int main()
{
	int p, g, a, b;

	long long int A, B, K;

	setlocale(LC_ALL, "rus");

	cout << "add p: ";
	cin >> p;
	cout << "add g: ";
	cin >> g;

	cout << "add a: ";
	cin >> a;
	cout << "add b: ";
	cin >> b;

	A = pow(g, a);
	A = A % p;
	B = pow(g, b);
	B = B % p;

	K = pow(A, b);
	K = K % p;

	cout << "you key: " << K << endl;

	system("pause");
	return 0;
}
