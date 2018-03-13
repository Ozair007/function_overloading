# function_overloading
#include <iostream>
#include <string>
#include <cmath>
using namespace std;
void smaller(string a, string b, string c);
void smaller(int a, int b, int c);
void smaller(double f1, double f2, double f3);
void saller(double a, double b, double c);
int main() {
	string a, b, c;
	a = "Syed";
	b = "Haroon";
	c = "Hameed";
	smaller(a, b, c);
	smaller(8, 4, 7);
	smaller(8.4345, 19.423, 12.64);
	smaller('a', 'b', 'c');
}
void smaller(string a, string b, string c) {
		int len_a = a.length();
		int len_b = b.length();
		int len_c = c.length();
		int smaller = len_a;
		if (len_a < len_b && len_a < len_c) {
			cout<<"A is smaller";
		}
		if (len_b < len_a && len_b < len_c) {
			cout<<"B is smaller";
		}
		if (len_c < len_a && len_c > len_a) {
			cout<<"C is smaller";
		}
		cout<<endl<<endl;
	}
void smaller(int a, int b, int c) {
	if (a < b && a < c) {
			cout<<"A is smaller";
		}
		if (b < a && b < c) {
			cout<<"B is smaller";
		}
		if (c < a && c > a) {
			cout<<"C is smaller";
		}
		cout<<endl<<endl;
}
void smaller(double f1, double f2, double f3) {
	if (f1 < f2 && f1 < f3) {
			cout<<"A is smaller";
		}
		if (f2 < f1 && f2 < f3) {
			cout<<"B is smaller";
		}
		if (f3 < f1 && f3 < f2) {
			cout<<"C is smaller";
		}
		cout<<endl<<endl;
}
