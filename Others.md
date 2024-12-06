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
