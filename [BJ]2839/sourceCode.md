    #include <iostream>
    using namespace std;
    int main() {
      int i;
      cin >> i;
      if (i == 4 || i == 7) 
        cout << "-1";
      else {
        if (i % 5 == 1 || i % 5 == 3)
          cout << (i / 5) + 1;
        else if (i % 5 == 2 || i % 5 == 4)
          cout << (i / 5) + 2;
        else
          cout << i / 5;
      }
    }


# [설명] 

설탕 배달은 5 또는 3 으로 만 나눌 수 있습니다. 계산을 해보면 
어떤 값 T를 받았을 때, 이를 5 로 나누면 몫이 나오게 되고
어떤 값 T를 받았을 때, 이를 5 로 % 연산하면 나머지가 나오게 됩니다.

이때 연산 관계를 나타내면 이렇게 볼 수 있습니다.

<img src="https://user-images.githubusercontent.com/39338850/63490968-f00ba180-c4f0-11e9-8d70-6449fc97e3bc.png" width="90%"></img>
