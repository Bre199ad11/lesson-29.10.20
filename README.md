#include <iostream>
using namespace std;

int f(int x) {
	int y = x * x;
	return y+1;
}

void procedure(int x) {
	cout << x << endl;
}
int main(){
	cout << f(13) << endl;
	procedure(42);
	int p=printf("%d %d %d\n", 1, 2, 3);
	cout << p << endl;
}
