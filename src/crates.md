# crates.io

From the official `cargo` book:

* [https://doc.rust-lang.org/cargo/reference/registries.html](https://doc.rust-lang.org/cargo/reference/registries.html)

> Running a Registry
>
> A minimal registry can be implemented by having a git repository that contains an index, and a server that contains the compressed .crate files created by cargo package. Users won't be able to use Cargo to publish to it, but this may be sufficient for closed environments.
>
> A full-featured registry that supports publishing will additionally need to have a web API service that conforms to the API used by Cargo. The web API is documented below.
>
> At this time, there is no widely used software for running a custom registry. There is interest in documenting projects that implement registry support, or existing package caches that add support for Cargo.

*Cargo* packages (*crates*) are `.crate` tarball files created by `cargo package`:

* [https://doc.rust-lang.org/cargo/commands/cargo-package.html](https://doc.rust-lang.org/cargo/commands/cargo-package.html)

Hosting a crates repository requires an implementation of `git-http-backend` such as:

* [https://git-scm.com/docs/git-http-backend](https://git-scm.com/docs/git-http-backend)

* [https://git-scm.com/book/en/v2/Git-on-the-Server-Smart-HTTP](https://git-scm.com/book/en/v2/Git-on-the-Server-Smart-HTTP)

Source Code from the ROMT project (Python):

* [romt/serve.py](https://github.com/drmikehenry/romt/blob/e71f709ee9ae0d3900c66954c1e69cb620d499f1/src/romt/serve.py)

Official `crates.io` repository index objects and refs on github: [https://github.com/rust-lang/crates.io-index](https://github.com/rust-lang/crates.io-index)

`git fetch https://github.com/rust-lang/crates.io-index`

ROMT main file: 
[https://github.com/drmikehenry/romt/blob/e71f709ee9ae0d3900c66954c1e69cb620d499f1/src/romt/cli.py](https://github.com/drmikehenry/romt/blob/e71f709ee9ae0d3900c66954c1e69cb620d499f1/src/romt/cli.py)
