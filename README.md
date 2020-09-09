![Algorythm of the night](https://github.com/massoprod/algorythm-of-the-night/blob/master/logo.png?raw=true)

# List of algorithms [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> Awesome list of algorithms that help you to solve your code issues or can help you in interviews if you are looking for a new job.

## Table of content
* [Factorial](#factorial)
* [Fibonacci](#fibonacci)
* [Includes](#includes)

## Algorithms

### Factorial
> The factorial function (symbol: !) says to multiply all whole numbers from our chosen number down to 1.
#### Example
`5! = 5 * 4 * 3 * 2 * 1 = 120`

#### Basic
```java
public static long factorial(int x) {
    long fact = 1;
    for (int i = 2; i <= x; i++) {
        fact = fact * i;
    }
    return fact;
}
```
#### Recursion
```java
public static long factorial(int x) {
    if (x == 0) {
        return 1;
    } else {
        return x * factorial(x - 1);
    }
}
```

### Fibonacci
> The Fibonacci series is a series of numbers in which each term is the sum of the two preceding terms. It's first two terms are 0 and 1.
#### Example
> The first 11 terms of the series are 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, and 55.

`S(n) = S(n-1) + S(n-2), with S(0) = 0 and S(1) = 1`

#### Recursion
```java
public static long fibonacci(int x) {
    if (x < 2) {
        return x;
    } else {
        return fibonacci(x-1) + fibonacci(x-2);
    }
}
```

### Includes
> Check if array of length *n* includes number *x*

> *left* and *right* are field boundaries

#### Recursion
```java
public static void includes(int [] array, int x, int left, int right) {
    if (left > right) {
        System.out.println("Not Includes");
    }

    if (array[left] == x) {
        System.out.println("Includes");
    } else {
        includes(array, x, left+1, right);
    }
}
```
