![Algorythm of the night](https://github.com/massoprod/algorythm-of-the-night/blob/master/logo.png?raw=true)

# List of algorithms [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> Awesome list of algorithms that help you to solve your code issues or can help you in interviews if you are looking for a new job.

## Table of content
1. Factorial
  * Recursive

## Algorithms

### Factorial
> The factorial function (symbol: !) says to multiply all whole numbers from our chosen number down to 1.
#### Recursive
```java
public static long factorial(int x) {
    if (x == 0) {
        return 1;
    } else {
        return x * factorialRecursive(x - 1);
    }
}
```
