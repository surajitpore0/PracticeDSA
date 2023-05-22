### Count digits in a number: 
```c++
int CountDigit(int number) {
	int count = 0;

	while (number != 0) {
		number = number / 10;
		count++;
	}

	return count;
}
```

### Reverse a Number:
```c++

long long ReverseNumber(long long number) {
	long long reverseNumber = 0;

	while (number != 0) {
		long long lastDigit = number % 10;
		reverseNumber = reverseNumber * 10 + lastDigit;
		number = number / 10;
	}

	return reverseNumber;
}

```

### Check if a number is Palindrome or Not:
```c++
int reverseNumber(int number) {
	int reverse = 0;

	while (number != 0) {
		int digit = number % 10;
		reverse = reverse * 10 + digit;
		number = number / 10;
	}

	return reverse;
}

bool IsPalindrome(int number) {
	if (reverseNumber(number) == number) {
		return true;
	}

	return false;
}
```

### GCD

**Brute force:**
```c++
int GCD (int a, int b) {
	int ans = 1;

	for (int i = 1; i <= min(a, b); i++) {
		if (a % i == 0 && b % i == 0) {
			ans = i;
		}
	}

	return ans;
}
```
