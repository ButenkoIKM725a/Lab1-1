# Lab1-1
#include <iostream>
#include <algorithm> 
using namespace std;
int main() {
    double a, b, c;
    cout << "Введіть три числа: ";
    cin >> a >> b >> c;

    double min1, min2;
    if (a >= b && a >= c) {
        min1 = b;
        min2 = c;
    } else if (b >= a && b >= c) {
        min1 = a;
        min2 = c;
    } else {
        min1 = a;
        min2 = b;
    }
    double diff1 = min1 - min2;
    cout << "Різниця двох найменших чисел: " << diff1 << endl;
    return 0;
}
