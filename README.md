x86 ASM development container
=============================

Vim is the editor installed with syntax highlighting via [vim-gas](https://github.com/Shirk/vim-gas/).
Source code is loaded in to the container via a volume.  Version control should be done outside of the container.

### Build the container

```
$ docker build -t justadam/asm-dev .
```

### Start the container

```
$ docker run -it --name asm-dev -v /path/to/src/:/workspace justadam/asm-dev
```

### Get back into the container

```
$ docker start -ai asm-dev
```
