已知`x`价值`75`, `y`价值`10`,  
需要的总价值为`115`, 那么只有一种可能`1*75+4*10`, 即`x+4y`.  
那么入参的`x`与`y`个数有`N`对`x+4y`, 则符合`N`轮, `N`为偶数(包括0, 即一轮也不符合)则赢的人为Bob, 为奇数则赢的人为Alice.
```java
    public static String losingPlayer(int x, int y) {
        int times = Math.min(x, y / 4);
        return times % 2 == 0 ? "Bob" : "Alice";
    }
```