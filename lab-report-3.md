# Lab Report 3

## Part 1 - Bugs

### Failure-inducing input
```
@Test
public void testReversedError() {
  int[] input1 = { 1, 2, 3 };
  assertArrayEquals(new int[] { 3, 2, 1 }, ArrayExamples.reversed(input1));
}
```
### Not failure-inducing input
```
@Test
public void testReversed() {
  int[] input1 = {};
  assertArrayEquals(new int[] {}, ArrayExamples.reversed(input1));
}
```

### Screenshots of symptom
![Image](lab-report-3-pics/symptom-test.png)

### Before bug fix
```
static int[] reversed(int[] arr) {
  int[] newArray = new int[arr.length];
  for(int i = 0; i < arr.length; i += 1) {
    arr[i] = newArray[arr.length - i - 1];
  }
  return arr;
}
```

### After bug fix
```
static int[] reversed(int[] arr) {
  int[] newArray = new int[arr.length];
  for (int i = 0; i < arr.length; i += 1) {
    newArray[i] = arr[arr.length - i - 1];
  }
  arr = newArray;
  return arr;
}
```

### Explanation for fix
By flipping which array the elements are reversed into and reversed from changed quite a few things. First of all, the new array has yet to be initialized with any data so by placing these values into the original array will result in an array full of zeroes. It's possible to avoid initializing the new array to be exactly the same as the original by instead adding the reversed elements into this new array. After doing this, the original array is set to the newly reversed array and this original array is returned with the reversed values.

## Part 2 - Researching Commands
