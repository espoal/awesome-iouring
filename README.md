# Awesome `io_uring` <a name="introduction"></a>
`io_uring` is considered one of the most revolutionary interfaces
for the linux kernel, [find out why]().

In this repository we try to collect examples, tutorials and
documentation about this amazing project, to raise awarness
and knowledge.

# Table of contents

1. [Introduction](#introduction)
2. [Tutorials](#Tutorials)
4. [Libraries](#Tutorials)
   - [C](#C) 
   - [C++](#C-1)
   - [Rust](#Rust)
   - [Golang](#Golang)
   - [Javascript](#Javascript)
   - [Python](#Python)

5. [Projects](#projects)
6. [Articles](#Articles)
7. [Other notable resources](#other)


## Tutorials
Tutorials about `io_uring`

- [Lord of the `io_uring`](https://unixism.net/loti/): Amazing collection of tutorials with deep explanations, 
unfortunately not updated often.

## Libraries 
Libraries for using `io_uring`

### C

- [liburing](https://github.com/axboe/liburing): Helper to interact with the kernel `io_uring` interface
- [xnvme](https://xnvme.io/): NVMe library with `io_uring` support
- [SPDK](https://spdk.io/): Intel library focused on performant io, with `io_uring` support

### C++

- [Seastar](https://github.com/scylladb/seastar): Asynchronous event-driven
  framework
- [liburing4cpp](https://github.com/CarterLi/liburing4cpp): Binding for `io_uring`
with coroutines support

### Rust

- [tokio-uring](https://github.com/tokio-rs/tokio-uring): An `io_uring` backend for `tokio`
- [io-uring](https://github.com/tokio-rs/io-uring): From the authors of `tokio`, without `tokio` dependency
- [rio](https://github.com/spacejam/rio): Pure rust `io_uring` library, unfortunately unmaintained 
- [Ringbahn](https://github.com/ringbahn/ringbahn): `io_uring` library from Berlin. Unfortunately unmaintained.

### Golang

- [gouring](https://github.com/ii64/gouring): Amazing `io_uring` library in pure golang


### Javascript

- [Bun](https://github.com/oven-sh/bun/blob/40eca63653db107fe69fd0208cc994b0d922070f/src/io/io_linux.zig#L530): Bun has support for `io_uring`
- [Nodejs](https://github.com/nodejs/node/issues/34388): Issue tracking `io_uring` support
- [Deno](https://github.com/denoland/deno/issues/16232): Issue tracking `io_uring` support

### Python

- [Liburing](https://github.com/YoSTEALTH/Liburing): Python bindings using CFFI
- [Metacall](https://github.com/metacall/python-c-io_uring-example): Example python bindings using `metacall`

### Ocaml

- [ocaml-uring](https://github.com/ocaml-multicore/ocaml-uring): `io_uring` bindings for OCaml


## Projects <a name="projects"></a>
Projects using `io_uring`

- [Glommio](https://github.com/DataDog/glommio)
- [Monoio](https://github.com/bytedance/monoio)
- [RocksDB](http://rocksdb.org/)
- [Bun](https://github.com/oven-sh/bun)
- [Scylladb](https://github.com/scylladb/scylladb)
- [Yottastore](https://github.com/yottaStore/yottaStore)

## Articles
Articles about `io_uring`

- [How io_uring and eBPF Will Revolutionize Programming in Linux](https://www.scylladb.com/2020/05/05/how-io_uring-and-ebpf-will-revolutionize-programming-in-linux/)

## Other notable resources <a name="other"></a>
Other resources about `io_uring`

- [IRC channel](https://webchat.oftc.net/?nick=amazingnickname&channels=%23io_uring&uio=d4): 
discussions about `io_uring`. You can find the archives [here](https://oftc.irclog.whitequark.org/io_uring/)
- [Mailing list](https://lore.kernel.org/io-uring/): The official dev mailing list of `io_uring`
- [Stackoverflow](https://stackoverflow.com/questions/tagged/io-uring): 
`io_uring` tagged questions and answers on stackoverflow