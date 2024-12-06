### Difference Between String, StringBuffer, and StringBuilder

| Feature                | String                        | StringBuffer                   | StringBuilder                  |
|------------------------|-------------------------------|---------------------------------|--------------------------------|
| **Mutability**         | Immutable                    | Mutable                        | Mutable                        |
| **Thread Safety**      | Not thread-safe              | Thread-safe (synchronized)     | Not thread-safe               |
| **Performance**        | Slower for modifications     | Slower due to synchronization  | Faster as it is not synchronized |
| **Usage**              | Used when string content is constant | Used in multithreading where thread safety is needed | Used for single-threaded applications requiring frequent modifications |
| **Method Efficiency**  | Every modification creates a new object | Operations are faster as it modifies the same object | Similar to StringBuffer but faster without synchronization |
| **Introduced In**      | JDK 1.0                      | JDK 1.0                        | JDK 1.5                        |
| **Example**            | `String s = "Hello";`        | `StringBuffer sb = new StringBuffer("Hello");` | `StringBuilder sb = new StringBuilder("Hello");` |



### Definitions of String, StringBuffer, and StringBuilder

- **String**:  
  A `String` in Java is an immutable sequence of characters. Once a `String` object is created, its value cannot be changed. Any modification, like appending or replacing, creates a new `String` object.

- **StringBuffer**:  
  A `StringBuffer` is a mutable sequence of characters. It allows modifications to its content without creating new objects. It is synchronized, making it thread-safe but slower in performance compared to `StringBuilder`.

- **StringBuilder**:  
  A `StringBuilder` is similar to `StringBuffer` as it is also mutable. However, it is not synchronized, meaning it is not thread-safe but offers better performance in single-threaded operations.
