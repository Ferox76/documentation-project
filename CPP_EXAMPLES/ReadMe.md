# C++ Examples

## Summation of two Integers

```c++
#include <iostream>


int add(int a, int b)
{
    return a + b;
}


int main()
{
    std::cout << "Summation of 2 integers" << std::endl;
    int a = 5;
    int b = 6;
    std::cout << "a + b = " << add(a, b) << std::endl;
    return 0;
}
```

## main with input parameters

```c++
#include <iostream>
#include <string>
using namespace std;

int main(int argc, char* argv[]) {

    int maxNo = 4;

    if (argc > maxNo + 1 ) {
        cout << "Bitte geben Sie maximal " << maxNo << " Zahlen an." << endl;
        return 1;
    }

   int summe = 0;
    for (int i = 1; i < argc; ++i) {
        int zahl = stoi(argv[i]);
        summe += zahl;
    }

    cout << "Die Summe der angegebenen Zahlen ist: " << summe << endl;
    return 0;
}
```