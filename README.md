CKB minimal UDT
===============

## Prepare

### Pull `ckb-riscv-gnu-toolchain` image

```
docker pull nervos/ckb-riscv-gnu-toolchain:xenial
```

## Develop

### Build

```
cd src
docker run --rm -it -v `pwd`:/code nervos/ckb-riscv-gnu-toolchain:xenial bash
root@3ede059e304b:/# cd /code
root@3ede059e304b:/code# riscv64-unknown-elf-gcc -Os udt.c -o udt
root@3ede059e304b:/code# exit
```
