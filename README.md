#include <iostream>
using namespace std;

int main() {
	int n;

	cout << "다이아몬드 크기를 입력하세요 : ";
	cin >> n;

	if (n <= 0) {
		cout << "잘못된 입력입니다." << endl;
		return 1;
	}
	for (int i = 0; i < n; i++) {
		for (int j = 0; j < n - i - 1; j++) {
			cout << " ";
		}
		for (int j = 0; j < 2 * i + 1; j++) {
			cout << "*";
		}
		cout << endl;
	}
	for (int i = n - 2; i >= 0; i--) {
		for (int j = 0; j < n - i - 1; j++) {
			cout << " ";
		}
		for (int j = 0; j < 2 * i + 1; j++) {
			cout << "*";
		}
		cout << endl;
	}


	return 0;
	
}
