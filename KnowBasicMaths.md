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