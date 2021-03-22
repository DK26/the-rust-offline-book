# Overview

Installing and using Rust within an online environment is very simple. All you have to do is download, install and use the `rustup` toolchain installer which sets everything that is required for the language to run. Then, you are using an internet connection to fetch crates from `crates.io` as you compile projects.

However, when it comes to an isolated computer that has no access to the internet, we will have to emulate all services offline for that same toolchain to function properly.  

The first step would be to download all these services' contents to a machine that has internet access, so we can provide them later offline.  

The second step is to serve all services locally either within a standalone machine or some other host within the isolated network.  

The third step is to configure your tools to work with the local services instead of the main official ones that otherwise could only be reached using an internet connection.

The fourth step is to configure your favorite Integrated Development Environment (IDE) to work with Rust offline.  

The tool `romt` seem to be a great tool to base the book on as it provides the steps between 1 and 3 and also provides support for updating the contents of the services incrementally.  

Other tools will be mentioned as well for different use-cases that may be resolved in different ways.  
