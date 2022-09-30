###  [Task 7kyu](https://www.codewars.com/kata/56269eb78ad2e4ced1000013/train/java)

You might know some pretty large perfect squares. But what about the NEXT one?

Complete the findNextSquare method that finds the next integral perfect square after the one passed as a parameter. Recall that an integral perfect square is an integer n such that sqrt(n) is also an integer.

If the parameter is itself not a perfect square then -1 should be returned. You may assume the parameter is non-negative.

### My solution
```Java
public class NumberFun {
    public static long findNextSquare(long sq) {
        long result;
        double d = Math.sqrt(sq);
        if ( d % 1 == 0) result = (long) Math.pow(++d, 2);
        else result = -1;
        return result;
    }
}
```

### Fav solution

```Java
public class NumberFun {
    public static long findNextSquare(long sq) {
        if((long)Math.sqrt(sq) != Math.sqrt(sq)) return -1;
        return sq+(2*(long)Math.sqrt(sq))+1;
    }
}

```
I like this solution because I like it
