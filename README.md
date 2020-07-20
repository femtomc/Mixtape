I am very inspired by the tooling in the [Julia language](https://julialang.org/) ecosystem for compiler interception and metaprogramming, which has allowed me to implement [a probabilistic programming library](https://github.com/femtomc/Jaynes.jl) in a concise and effective way.

One limitation of `Julia` is the inability to distribute portable binaries of source code - requiring that a local machine have access to the Julia JIT compiler (similar to how language-based VMs require a local VM to function, unless static compilation to native is supported).

With this in mind, I've begun to experiment with LLVM - in the hopes that a similar form of tracing/metaprogramming functionality can be utilized in other LLVM-based language impementations.
