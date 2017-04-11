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
#### Cek Palindrome
```
boolean checkPalindrome(String inputString) {
    return inputString.equals(new StringBuffer(inputString).reverse().toString());
}
```
#### Mencari nilai terbesar/terkecil dalam List
```
Collections.max(<List>)
```
###### Contoh pemakaian
```
int adjacentElementsProduct(int[] inputArray) {
    List<Integer> result = new ArrayList<>();
    for (int i = 0; i < inputArray.length - 1; i++) {
        result.add(inputArray[i] * inputArray[i + 1]);
    }
    return (int) Collections.max(result);
}
```
