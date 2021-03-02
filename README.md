# OS : Operating-System

OS is a very simple operating system from scratch with a x86 Architecture and mutliboot2 system.

## Contributing

- Thomas Chastaingt

### Requirements

Make sure the following dependencies are installed:
- [Docker](https://www.docker.com/)
- [Qemu](https://www.qemu.org/)


### Running



Start :
```bash
$ docker build buildenv -t myos-buildenv
$ docker run --rm -it -v "$PWD":/root/env myos-buildenv
$ make build-x86_64
leave VM:
$ qemu-system-x86_64 -cdrom dist/x86_64/kernel.iso

```

## Codebase

#### Technologies
Here is a list of all the big technologies we use:

    - Assembly
    - Makefile
    - C


