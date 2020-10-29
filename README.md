#include <iostream>
using namespace std;
#include <ctime>

int f(int x) {
	int y = x * x;
	return y+1;
}

void procedure(int x) {
	cout << x << endl;
}
int main(){
	srand(time(0));
	cout << f(13) << endl;
	procedure(42);
	int p=printf("%d %d %d\n", rand()%100, rand() % 100, rand() % 100);
	cout << p << endl;
}
