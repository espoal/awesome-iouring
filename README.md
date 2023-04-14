# Awesome `io_uring` <a name="introduction"></a> [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

`io_uring` is considered one of the most revolutionary interfaces
for the linux kernel, [find out why](https://www.scylladb.com/2020/05/05/how-io_uring-and-ebpf-will-revolutionize-programming-in-linux/).

In this repository we try to collect tutorials, articles, examples  and
documentation about this amazing project, to raise awareness
and knowledge.

## Highlights

hello

// TODO: add some highlights
// TODO: sort languages by use

# Table of contents

1. [Introduction](#introduction)

2. [Content](#content)
   - [Articles](#Articles)
   - [Videos](#Videos)
   - [Tutorials](#tutorials)
   
3. [Libraries](#Libraries)
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

4. [Projects](#projects)
   - [Databases](#Databases)
   - [Storage engines](#storage)
   - [Network](#network)
   - [Other](#other)
   

7. [Other notable resources](#other)

# Content
Content about `io_uring`, ordered by timestamp descending.

## Articles

- [Why you should use `io_uring`](https://developers.redhat.com/articles/2023/04/12/why-you-should-use-iouring-network-io)
- [Efficient IO with `io_uring`](https://kernel.dk/io_uring.pdf)
- [Ringing in a new asynchronous I/O API](https://lwn.net/Articles/776703/)
- [How io_uring and eBPF Will Revolutionize Programming in Linux](https://www.scylladb.com/2020/05/05/how-io_uring-and-ebpf-will-revolutionize-programming-in-linux/)
- [Experiments with io_uring](https://blog.virtual-void.net/2022/10/11/experiments-with-io-uring/)
- [IO_uring Fixed Buffer Versus Non-Fixed Buffer Performance Comparison on NVMe](https://00pauln00.medium.com/io-uring-fixed-buffer-versus-non-fixed-buffer-performance-comparison-9fd506de6829)
- [Missing manuals - io_uring worker pool](https://blog.cloudflare.com/missing-manuals-io_uring-worker-pool/)
- [io_uring in Android OTA](https://lpc.events/event/16/contributions/1331/attachments/951/1867/LPC2022%20-%20io_uring%20in%20Android%20OTA.pdf): Linux plumbers conference 2022 presentation
- [A journey to io_uring, AIO and modern storage devices](https://clickhouse.com/blog/a-journey-to-io_uring-aio-and-modern-storage-devices): includes experiments on Optane storage

- 2023-04 [Why you should use io_uring for network I/O](https://developers.redhat.com/articles/2023/04/12/why-you-should-use-iouring-network-io)
- 2023-02 [io_uring and networking in 2023](https://github.com/axboe/liburing/wiki/io_uring-and-networking-in-2023)
- 2022-03 [IO_uring Gets New Features & Speed-Ups With Linux 5.18](https://www.phoronix.com/scan.php?page=news_item&px=Linux-5.18-IO_uring)
- 2022-03 [Put an io_uring on it: Exploiting the Linux Kernel](https://www.graplsecurity.com/post/iou-ring-exploiting-the-linux-kernel)
- 2022-02 [Missing Manuals - io_uring worker pool](https://blog.cloudflare.com/missing-manuals-io_uring-worker-pool/)
- 2021-12 [Zero-copy network transmission with
  io_uring](https://lwn.net/Articles/879724/)
- 2021-10 [Stupid tricks with io_uring: a server that does zero syscalls per
  request](https://wjwh.eu/posts/2021-10-01-no-syscall-server-iouring.html)
- 2021-06 [io_uring is not an event
  system](https://despairlabs.com/posts/2021-06-16-io-uring-is-not-an-event-system/)
- 2021-05 [Using io_uring to make a high-performance... finger server](https://drewdevault.com/2021/05/24/io_uring-finger-server.html)
- 2021-03 [I made a file copy thing](https://wheybags.com/blog/wcp.html)
- 2020-05 [Notes on io-uring](https://boats.gitlab.io/blog/post/io-uring/)
- 2020-05 [How io_uring and eBPF Will Revolutionize Programming in
  Linux](https://www.scylladb.com/2020/05/05/how-io_uring-and-ebpf-will-revolutionize-programming-in-linux/)
- 2020-04 [io_uring by
  example](https://unixism.net/2020/04/io-uring-by-example-article-series/)
- 2019-01 [Ringing in a new asynchronous I/O
  API](https://lwn.net/Articles/776703/)




## Videos

- [Understanding Modern Storage APIs: A systematic study of libaio, SPDK, and io_uring](https://www.youtube.com/watch?v=5jKKVdJJqKY)
- 2022-06 [What's new with io_uring?](https://youtu.be/v--rVT4RsCE?t=2045) ([Slides](https://kernel.dk/axboe-kr2022.pdf))

## Tutorials and documentation <a name="tutorials"></a>
Tutorials about `io_uring`

- [io_uring and networking in 2023](https://kernel.dk/io_uring%20and%20networking%20in%202023.pdf): tutorial written by Jens Axboe, the creator of `io_uring`
* [io_uring manpage](https://www.mankier.com/7/io_uring)
* [Lord of the io_uring](https://unixism.net/loti/) - a guide to using io_uring

### C

- [Lord of the `io_uring`](https://unixism.net/loti/): Amazing collection of tutorials with deep explanations,
  unfortunately not updated often.

### Zig

- [Building a high-performance database buffer pool in Zig using io_uring's new fixed-buffer mode](https://gavinray97.github.io/blog/io-uring-fixed-bufferpool-zig)


# Libraries 
Libraries for using `io_uring`

### C

- [liburing](https://github.com/axboe/liburing): Helper to interact with the kernel `io_uring` interface
- [xnvme](https://xnvme.io/): NVMe library with `io_uring` support
- [SPDK](https://spdk.io/): Intel library focused on performant io, with `io_uring` support
- [libev](https://github.com/hanyong/libev): High performance event loop

* [libfev](https://github.com/patrykstefanski/libfev) - A library for events and
  fibers
* [liburing](https://github.com/axboe/liburing/) - wrapper lib for io_uring by
  [io_uring's author](https://github.com/axboe)
* [PhotonLibOS](https://github.com/alibaba/PhotonLibOS) - a high-efficiency LibOS framework, based on a set of carefully selected C++ libs.
* [xynet](https://github.com/xuanyi-fu/xynet) - network library based on
  io_uring and C++20 coroutine

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
- [rio](https://github.com/spacejam/rio): Pure rust `io_uring` library, unfortunately unmaintained 
- [Ringbahn](https://github.com/ringbahn/ringbahn): `io_uring` library from Berlin. Unfortunately unmaintained.

* [glommio](https://github.com/DataDog/glommio) - a Cooperative Thread-per-Core
  crate for Rust & Linux based on io_uring
* [io-uring](https://github.com/tokio-rs/io-uring) - The io_uring library for
  Rust
* [Monoio](https://github.com/bytedance/monoio) - a thread-per-core Rust runtime
  with io_uring
* [nuclei](https://github.com/vertexclique/nuclei) - Proactive IO & Runtime system
* [ringbahn](https://github.com/ringbahn/ringbahn) - safe bindings to io_uring
* [rio](https://github.com/spacejam/rio) - pure rust io_uring library, built on
  libc, thread & async friendly, misuse resistant

### Golang

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

* [io_uring-java](https://github.com/ChinaXing/io_uring-java) - Java binding for
  io_uring
* [Jliburing](https://github.com/Sammers21/Jliburing) - Java binding for
  liburing and io_uring

### Kotlin

- [kuring](https://github.com/ikorennoy/kuring): Async io library

### Ocaml

- [ocaml-uring](https://github.com/ocaml-multicore/ocaml-uring): `io_uring` bindings for OCaml

### Lua

* [Luring](https://github.com/thislight/luring) - a callback-style interface for
  Lua to io_uring

### .NET

* [IoUring](https://github.com/tkp1n/IoUring) - `io_uring` wrapper for C# / .NET

### Python

* [Liburing](https://github.com/YoSTEALTH/Liburing) - a Python + CFFI wrapper
  around the liburing C library


### Ruby

* [io-event](https://github.com/socketry/io-event/) - Fiber scheduler for Ruby 3.0
* [polyphony](https://github.com/digital-fabric/polyphony) - Fiber-based
  concurrency for Ruby using io_uring

# Projects 
Projects using `io_uring`

### Databases

- [ClickHouse](https://github.com/ClickHouse/ClickHouse)
- [Postgres](https://github.com/anarazel/postgres/tree/aio) (experimental)
- [questdb](https://github.com/questdb/questdb)
- [Scylladb](https://github.com/scylladb/scylladb)
- [Yottastore](https://github.com/yottaStore/yottaStore)

### Datastores

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

* [Cachegrand](https://github.com/danielealbano/cachegrand) - an open-source
  fast, scalable and secure Key-Value
* [Dragonfly](https://github.com/dragonflydb/dragonfly) - A modern replacement for Redis and Memcached
* [plocate](https://plocate.sesse.net/) - a much faster `locate` using io_uring
* [Short-circuit](https://github.com/3541/short-circuit) - High-performance web
  server for Linux, built on io_uring
* [wcp](https://github.com/wheybags/wcp) - Copy files very fast using io_uring



# Other notable resources <a name="other"></a>
Other resources about `io_uring`

- [IRC channel](https://webchat.oftc.net/?nick=amazingnickname&channels=%23io_uring&uio=d4): 
discussions about `io_uring`. You can find the archives [here](https://oftc.irclog.whitequark.org/io_uring/)
- [Mailing list](https://lore.kernel.org/io-uring/): The official dev mailing list of `io_uring`
- [Stackoverflow](https://stackoverflow.com/questions/tagged/io-uring): 
`io_uring` tagged questions and answers on stackoverflow

### Related lists

Other amazingly awesome lists can be found in the
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
list.

## License

[![CC0](https://i.creativecommons.org/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Alberto Esposito](http://github.com/espoal) has
waived all copyright and related or neighboring rights to this work.
