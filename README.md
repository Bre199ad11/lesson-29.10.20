#include <iostream>
using namespace std;

int f(int x) {
	int y = x * x;
	return y+1;
}

int main(){
	cout << f(13) << endl;
}
