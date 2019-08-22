	#include <iostream>
	#include <algorithm>
	using namespace std;


	int main() {
		int T,NOW = 0,MAX;
		cin >> T;
		int* arr = new int[T];

		for (int i = 0; i < T; ++i) {
			cin >> arr[i];
			NOW += arr[i]; // i번째에 있는 값을 NOW 에 누적시킴
			if (!i) // i 가 0번째라면 최댓값은 arr[0] 값이 됨
				MAX = arr[i];

			else // 아니라면 최댓값은 MAX 와 NOW 중 더 큰 것을 고름
				MAX = max(MAX, NOW);

			if (NOW < 0)
				NOW = 0;  
		}
			cout << MAX << endl;
			delete[] arr;
	}
