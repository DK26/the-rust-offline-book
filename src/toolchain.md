# Offline Toolchain

In order to acquire the Rust toolchain for offline usage, we will be using the `romt` tool.

`romt` is an open-source tool that was created by _Michael Henry_ and was written in Python (see _Available Tools_ section for more details).  

This tool enables us to acquire all contents from each service in the rustup toolchain and host these services locally.

The next steps will describe what needs to be done to acquire and setup both the _rustup toolchain_ for offline usage and a _local repository_ for our crates, instead of the default _crates.io_ one.  

Then, we will see how to configure _cargo_ to work with it globally.

> A computer with access to the internet is required to acquire and validate all resources.  

Also, the next tools are _required_ for the book. Download the proper versions required by your environment.

| Required | Description | Download Page |
| -------- | ------------- | ----------- |
| `romt` | A compiled version of the `romt` command line tool | [https://github.com/drmikehenry/romt/releases](https://github.com/drmikehenry/romt/releases) |
| `git` | _Required_ by `romt` | [https://git-scm.com/downloads](https://git-scm.com/downloads) |
| `gpg` | Used by `romt` to verify the downloaded contents (_Highly Recommended_) | [https://gnupg.org/download/index.html](https://gnupg.org/download/index.html) |  

> **FOR LINUX USERS**  
> Installing the tools here in your environment may be done differently. In the future, I hope to provide a linux section.  
>
> _Feel free to contribute!_  
