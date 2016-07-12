# programming-cheat-sheet
Beberapa contekan untuk programming contest

#### Cara cepat menentukan bilangan prima
```
bool isPrime(int num) {
    if (num == 1) {
        return false;
    }
    if (num == 2) {
        return true;
    }
    if (num%2 == 0) {
        return false;
    }
    for (int i = 3; i <= sqrt(num); i+=2) {
        if (num%i == 0) {
            return false;
        }
    }
    return true;
}
```
