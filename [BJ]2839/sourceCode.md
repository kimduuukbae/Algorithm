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
