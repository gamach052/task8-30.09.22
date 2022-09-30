###  [Task 7kyu](https://www.codewars.com/kata/56269eb78ad2e4ced1000013/train/java)

Complete the function that calculates the area of the red square, when the length of the circular arc A is given as the input. Return the result rounded to two decimals.
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
