#include <iostream>

using namespace std;

#include <ctime>

/*int f(int x) {
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
	cout << p << endl;*/


template <typename T> 

void print_a(T* array, int size) {
	for (int i = 0; i < size; i++) {
		cout << array[i] << ' ';
	}
	cout << endl;
}

template <typename T>

void bubble_sort(T* array, int size){
	for (int i = size; i >= 0; i--) {
		for (int j = 0; j < i - 1; j++) {
			if (array[j] > array[j + 1]){
				T temp =array[j];
				array[j]=array[j+1];
				array[j+1]=temp;
			}
		}
	}
}


int main() {
	int a[] = { 1,4,5,7,2,6,9,8,3 };
	bubble_sort(a, 9);
	print_a(a, 9);
	double b[] = { 6,7,4,5,3,2,8,1,3,9,10 };
	bubble_sort(b, 11);
	print_a(b, 11);
	
}
