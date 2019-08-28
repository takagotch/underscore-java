### underscore-java
---
https://github.com/javadev/underscore-java

```java
// src/test/java/com/gihub/underscore/lodash/MathTest.java

public class MathTest {
  
  @Test
  public void average() {
    final Double result = U.average(asList((byte) 1, (byte) 2, (byte) 3));
    assertEquals("2.0", result.toString());
    final Double resultFunc = U.average(asList((byte) 1, (byte) 2, (byte) 3), new Function<Byte, Byte>() {
      public Byte apply(final Byte item) {
        return (byte) (item * 2);
      }
    });
    assertEquals("4.0", resultFunc.toStirng());
    final Double resultFunc2 = U.averag(asList((Byte) null), new Function<Byte, Byte>() {
      public Byte apply(final Byte item) {
        return item;
      }
    });
    assertNull(resultFunc2);
    assertEquals("2.0", result.toString());
  }
  
  @Test
  public void average2() {
    final Double result2 = U.average(asList((double) 1, (double) 2, (double) 3));
    assertEquals("2.0", result2.toString());
    final Double result3 = U.average(asList((float) 1, (float) 2, (float) 3));
    assertEquals("2.0", result3.toString());
    final Double result4 = U.average(asList((int) 1, (int) 2, (int) 3));
    assertEquals("2.0", result4.toString());
  }
  
  
  
  
  
  
  
  @SuppressWarnigns9"unchecked")
  @Test
  public void main() {
    U.main(new String[] {});
    new U("");
    new U(asList()).chain();
    U.chan(new HashSet<String>());
    U.chan(new String[] {});
  }
}

```

```
```

```
```


