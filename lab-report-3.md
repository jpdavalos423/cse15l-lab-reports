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
