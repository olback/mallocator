# Mallocator

```rust
#![no_std]
#![feature(default_alloc_error_handler)]

use mallocator::Mallocator;

#[global_allocator]
static A: Mallocator = Mallocator;

fn my_fn_that_requires_heap() {
    let v = vec![1, 2, 3];
}
```

