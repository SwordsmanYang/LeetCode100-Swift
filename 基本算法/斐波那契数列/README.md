# Fibonacci （斐波那契数列实现）



## From

《剑指offer》Question No.9



## Question

Code implementation of fibonacci.


## Solution  



### Swift
```swift
func fib(_ N: Int) -> Int {
    if N <= 0 {
        return 0
    }
    
    var first = 0
    var second = 1
    
    for _ in 0 ..< (N - 1) {
        let sum = first + second
        
        first = second
        second = sum
    }

    return second
}
```





