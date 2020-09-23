# devtoolset-3

Packages to downgrade the gcc compiler version to 4.9.2 in Fedora.

## Steps
```
  $ git clone https://github.com/leylandcn/centos-7-gcc.git
  $ cd centos-7-gcc
  $ yum -y install dnf
  $ dnf install ./*.rpm
  $ scl enable devtoolset-3 bash
```

**NOTE:** Be aware that the command `scl enable devtoolset-3 bash` enables gcc/g++ v4.9 in the current terminal session only.

**NOTE:** Modify ~/.bashrc

source scl_source enable devtoolset-3
