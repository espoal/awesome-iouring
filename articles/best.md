# Best practices for using `io_uring`

- Use fixed buffers when possible
- Implement syscalls with `io_uring`, not only `read` and `write` but also `open`, ...
- When doing multithreaded programming, prefer to use one ring per thread, and 
leave synchronization to the kernel 

## Implementation tips


- If you're doing Go/Rust, consider using syscalls instead 
of implementing unsafe `liburing`
- Remember to use a recent kernel (6.0+)
