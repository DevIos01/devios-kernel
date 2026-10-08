# devios-kernel

Built releases of the C# kernel that runs DevIos IDE sessions on [devios.dev/ide](https://www.devios.dev/ide).
The kernel is Roslyn on a .NET 10 WebAssembly runtime, compiled to a static bundle that the browser downloads.

This repository holds **release assets only**. Each release is tagged `kernel-<hash>`, where the hash is
taken over the kernel's source inputs. The devios.dev build downloads the release whose hash matches the
source it is building, so a deploy always ships the engine its code was written against.

The same files are served publicly from `https://www.devios.dev/kernel/` once deployed.
