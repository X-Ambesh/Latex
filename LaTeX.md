C++  important questions 

### Write a code to print sum of even digits and product of odd digits of a number.

```
#include <iostream>
using namespace std;
int main() {
    int num;
    cout << "Enter a number: ";
    cin >> num;
    int even =0;
    int odd =1;
    while (num > 0) {
        int digit = num % 10;
        if (digit % 2 == 0) {
            even += digit;
        }
        else {
            odd *= digit;
        }
        num /= 10;
    }
    cout << "Sum of even digits:  " << even << endl; ;
    cout << "Product of odd digits:  " << odd << endl;
    return  0;
}
```
###  To print factorial of a number .
   
```
  #include <iostream>
using namespace std;
int main() {
    int num;
    cout << "Enter a number: ";
    cin >> num;
    int fac=1;
    for(int i=1; i<=num; i++)
        fac *= i;
    cout << "Factorial of " << num << " is: " << fac << endl;
    return 0;
} 
```
### To reverse a number 
```
#include <iostream>
using namespace std;
int main() {
    int num;
    cout << "Enter a number: ";
    cin >> num;
    int rev=0;
    while (num > 0) {
        rev = rev * 10 + num % 10;
        num /= 10;
    }
    cout << "Reversed number: " << rev << endl;
    return 0;
}
```

### To check weather a number is palidrome or not 

```
#include <iostream>
using namespace std;
int main() {
    int num;
    cout << "Enter a number: ";
    cin >> num;
    int rev = 0;
    while (num > 0) {
        rev = rev * 10 + num % 10;
        num /= 10;
    }
    if (rev == num) {
        cout << "The number is a palindrome." << endl;
    } else {
        cout << "The number is not a palindrome." << endl;
    }
    return 0;
}
```
### To check weather a number is prime or not 

```
#include <iostream>
using namespace std;
int main() {
    int num;
    cout << "Enter a number: ";
    cin >> num;
    int p = 0;
    for (int i = 1; i <= num; i++) {
        if (num % i == 0) {
        p += 1;}
    }
    if (p > 2) {
        cout << "The number is not prime." << endl;
    } else {
        cout << "The number is prime." << endl;
    }
    return 0;
}
```