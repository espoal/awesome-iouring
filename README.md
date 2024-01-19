# Awesome `io_uring` <a name="introduction"></a>
`io_uring` is considered one of the most revolutionary interfaces
for the linux kernel, [find out why](https://www.scylladb.com/2020/05/05/how-io_uring-and-ebpf-will-revolutionize-programming-in-linux/).

In this repository we try to collect examples, tutorials and
documentation about this amazing project, to raise awarness
and knowledge.

# Table of contents

1. [Introduction](#introduction)
2. [Tutorials](#Tutorials)
4. [Libraries](#Tutorials)
   - [C](#C) 
   - [C++](#C-1)
   - [D](#D)
   - [Rust](#Rust)
   - [Golang](#Golang)
   - [Javascript](#Javascript)
   - [Python](#Python)
   - [Java](#Java)
   - [Kotlin](#Kotlin)
   - [OCaml](#OCaml)

5. [Projects](#projects)
   - [Databases](#Databases)
   - [Storage engines](#storage)
   - [Network](#network)
   - [Other](#other)
   
6. [Articles](#Articles)
7. [Videos](#Videos)
8. [Other notable resources](#other)


## Tutorials
Tutorials about `io_uring`

- [io_uring and networking in 2023](https://kernel.dk/io_uring%20and%20networking%20in%202023.pdf): tutorial written by Jens Axboe, the creator of `io_uring`

### C

- [Lord of the `io_uring`](https://unixism.net/loti/): Amazing collection of tutorials with deep explanations, 
unfortunately not updated often.

### Zig

- [Building a high-performance database buffer pool in Zig using io_uring's new fixed-buffer mode](https://gavinray97.github.io/blog/io-uring-fixed-bufferpool-zig)


## Libraries 
Libraries for using `io_uring`

### C

- [liburing](https://github.com/axboe/liburing): Helper to interact with the kernel `io_uring` interface
- [xnvme](https://xnvme.io/): NVMe library with `io_uring` support
- [SPDK](https://spdk.io/): Intel library focused on performant io, with `io_uring` support
- [libev](https://github.com/hanyong/libev): High performance event loop

### C++

- [Seastar](https://github.com/scylladb/seastar): Asynchronous event-driven
  framework
- [liburing4cpp](https://github.com/CarterLi/liburing4cpp): Binding for `io_uring`
with coroutines support
- [ubdsrv](https://github.com/ming1/ubdsrv): Userspace block device driver
using `io_uring`
- [libunifex](https://github.com/facebookexperimental/libunifex): Facebook prototype for cpp async 
programming model

### D

- [during](https://github.com/tchaloupka/during): An `io_uring` implementation in pure Dlang

### Rust

- [tokio-uring](https://github.com/tokio-rs/tokio-uring): An `io_uring` backend for `tokio`
- [io-uring](https://github.com/tokio-rs/io-uring): From the authors of `tokio`, without `tokio` dependency
- [nuclei](https://github.com/vertexclique/nuclei): Reactor agnostic Proactive IO engine using `io_uring`
- [compio](https://github.com/compio-rs/compio): A single threaded async runtime using `io_uring` on Linux if available.
- [rio](https://github.com/spacejam/rio): Pure rust `io_uring` library, unfortunately unmaintained 
- [Ringbahn](https://github.com/ringbahn/ringbahn): `io_uring` library from Berlin. Unfortunately unmaintained.

### Golang

- [gain](https://github.com/pawelgaczynski/gain) - A high-performance, lightweight `io_uring` networking framework written entirely in Go.
- [gouring](https://github.com/ii64/gouring): Amazing `io_uring` library in pure golang
- [iouring-go](https://github.com/Iceber/iouring-go): Async interface for `io_uring`

### Javascript

- [Bun](https://github.com/oven-sh/bun/blob/40eca63653db107fe69fd0208cc994b0d922070f/src/io/io_linux.zig#L530): Bun has support for `io_uring`
- [Nodejs](https://github.com/nodejs/node/issues/34388): Issue tracking `io_uring` support
- [Deno](https://github.com/denoland/deno/issues/16232): Issue tracking `io_uring` support

### Python

- [Liburing](https://github.com/YoSTEALTH/Liburing): Python bindings using CFFI
- [Metacall](https://github.com/metacall/python-c-io_uring-example): Example python bindings using `metacall`

### Java

- [Jasyncfio](https://github.com/ikorennoy/jasyncfio): Async io library
- [nio_uring](https://github.com/bbeaupain/nio_uring): Async io library
- [Netty transport](https://github.com/netty/netty-incubator-transport-io_uring)
- [PanamaUring](https://github.com/dreamlike-ocean/PanamaUring) :Use java Panama ffi api to provide io_uring binding for java without using jni binding, while unifying the models of file IO and network IO, and providing an easy-to-use asynchronous IO API

### Kotlin

- [kuring](https://github.com/ikorennoy/kuring): Async io library

### Ocaml

- [ocaml-uring](https://github.com/ocaml-multicore/ocaml-uring): `io_uring` bindings for OCaml


## Projects 
Projects using `io_uring`

### Databases

- [ClickHouse](https://github.com/ClickHouse/ClickHouse)
- [Postgres](https://github.com/anarazel/postgres/tree/aio) (experimental)
- [questdb](https://github.com/questdb/questdb)
- [Scylladb](https://github.com/scylladb/scylladb)
- [Yottastore](https://github.com/yottaStore/yottaStore)

### Storage engines <a name="storage"></a>

- [Glommio](https://github.com/DataDog/glommio)
- [Monoio](https://github.com/bytedance/monoio)
- [RocksDB](http://rocksdb.org/)
- [Tigerbeetle](https://github.com/tigerbeetledb/tigerbeetle)
- [Ceph](https://github.com/ceph/ceph)
- [Samba](https://www.snia.org/educational-library/samba-multi-channel-iouring-status-update-2021)

### Network

- [Netty](https://github.com/netty/netty-incubator-transport-io_uring)
- [Zuul](https://github.com/Netflix/zuul)


### Other

- [QEMU](https://wiki.qemu.org/Features/IOUring)
- [Bun](https://github.com/oven-sh/bun)


## Articles
Articles about `io_uring`

- [Why you should use `io_uring`](https://developers.redhat.com/articles/2023/04/12/why-you-should-use-iouring-network-io)
- [Efficient IO with `io_uring`](https://kernel.dk/io_uring.pdf)
- [Ringing in a new asynchronous I/O API](https://lwn.net/Articles/776703/)
- [How io_uring and eBPF Will Revolutionize Programming in Linux](https://www.scylladb.com/2020/05/05/how-io_uring-and-ebpf-will-revolutionize-programming-in-linux/)
- [Experiments with io_uring](https://blog.virtual-void.net/2022/10/11/experiments-with-io-uring/)
- [IO_uring Fixed Buffer Versus Non-Fixed Buffer Performance Comparison on NVMe](https://00pauln00.medium.com/io-uring-fixed-buffer-versus-non-fixed-buffer-performance-comparison-9fd506de6829)
- [Missing manuals - io_uring worker pool](https://blog.cloudflare.com/missing-manuals-io_uring-worker-pool/)
- [io_uring in Android OTA](https://lpc.events/event/16/contributions/1331/attachments/951/1867/LPC2022%20-%20io_uring%20in%20Android%20OTA.pdf): Linux plumbers conference 2022 presentation
- [A journey to io_uring, AIO and modern storage devices](https://clickhouse.com/blog/a-journey-to-io_uring-aio-and-modern-storage-devices): includes experiments on Optane storage

## Videos

- [Understanding Modern Storage APIs: A systematic study of libaio, SPDK, and io_uring](https://www.youtube.com/watch?v=5jKKVdJJqKY)

## Other notable resources <a name="other"></a>
Other resources about `io_uring`

- [IRC channel](https://webchat.oftc.net/?nick=amazingnickname&channels=%23io_uring&uio=d4): 
discussions about `io_uring`. You can find the archives [here](https://oftc.irclog.whitequark.org/io_uring/)
- [Mailing list](https://lore.kernel.org/io-uring/): The official dev mailing list of `io_uring`
- [Stackoverflow](https://stackoverflow.com/questions/tagged/io-uring): 
`io_uring` tagged questions and answers on stackoverflow
