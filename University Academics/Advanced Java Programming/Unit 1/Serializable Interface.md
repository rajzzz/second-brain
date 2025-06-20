A marker [[Interface]] used to indicate that a class's objects can be converted into a byte stream.
This lets them to be:
- Saved to a file
- Transferred over a network
- Stored in memory

The process is called serialization, and converting the byte stream back into an object is called deserialization.

**Package:** `java.io.Serializable`

#### Making a Class Serializable:
```java
import java.io.Serializable;

public class Student implements Serializable {
  private int id;
  private String name;

  // constructor, getters, setters...
}
```
