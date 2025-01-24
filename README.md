# cs121_2025__project_2__bubble_sort
A Bubble Sorter checks for the largest number that is out of place, then compares it to the surrounding numbers, until it is in the correct spot

### Starter Code - 
```
#include <stdio.h>
const int MAX=9;

void printValues(int*);
void sort(int*);
void swap(int*, int*);

int main(){
  int values[] = {7, 3, 9, 4, 6, 1, 2, 8, 5};
  printf("Before: \n");
  printValues(values);

  // test swap
  int x = 3;
  int y = 5;
  printf("x: %d, y: %d \n", x, y);
  swap(&x, &y);
  printf("x: %d, y: %d \n", x, y);

  sort(values);
  printf("After: \n");
  printValues(values);

  return(0);
} // end main
```
### Include and Variables
```
include Input Output
Create Const MAX
Create Pointer lower
Create Pointer higher
```
### Main() 
```
print original array
call function PrintValues()
call function Sort()
call function Swap()
return 0
print final array
```

### PrintValues()
```
//print value of array
take int pointer for array and const for MAX
	for i of array from 0 to MAX, i ++;
		print value of i
do not return anything (already a void)
```

### Sort()
```
use bubble sort on array
constant MAX is max length of array
function sort (array):
    create integer variables i and j
    for i from zero to MAX - 1:
        for j from zero to MAX - 1:
            if array[j] > array[j+1]:
                swap array[j] with array[j+1]
                printArray(array)
do not return anything (already a void)
```

### Swap()
```
take pointer values lower and higher
Create pointer temp
copy the value of lower to temp
copy the value of higher to lower
copy the value of temp to higher
do not return anything (already a void)
```
.
