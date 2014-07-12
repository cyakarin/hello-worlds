## Environment
* OS: CentOS6.5
* Kernel: 2.6.32-431.el6.x86_64

## Dependencies
* glibc-devel(x86_64 x86_32)
* libgcc-devel(x86_64 x86_32)

    ```
    $ sudo yum install glibc-devel libgcc-devel glibc-devel.i686 libgcc-devel.i686
    ```

## Getting Started
* Install compiler

    ```
    $ wget http://downloads.dlang.org.s3-website-us-east-1.amazonaws.com/releases/2013/dmd-2.063.2-0.fedora.x86_64.rpm ~/download/compiler
    $ sudo rpm -ivh ~/download/compiler/dmd-2.063.2-0.fedora.x86_64.rpm
    ```

* Excute

    ```
    $ rdmd hello_world.d
    ```
