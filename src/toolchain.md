# Offline Toolchain

In order to acquire the Rust toolchain for offline usage, we will be using the `romt` tool.

`romt` is an open-source tool that was created by _Michael Henry_ and was written in Python (see _Tools_ section for more details).  

This tool enables us to acquire all contents from each service in the rustup toolchain and host these services locally.

The next steps will describe what needs to be done to acquire and setup both the _rustup toolchain_ for offline usage and a _local repository_ for our crates, instead of the default _crates.io_ one.  

Then, we will see how to configure _cargo_ to work with it globally.

> ### Requirements
> A computer with access to the internet is required to acquire and validate all resources.  
>
> You can download a compiled version of the `romt` command line tool from https://github.com/drmikehenry/romt/releases
