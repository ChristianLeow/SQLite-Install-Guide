# SQLite Install Guide

[TOC]

This document will guide you through the installation of SQLite on Ubuntu 18.04 LTS x64.



## Install via `apt`

If you are comfortable with the official release version of SQLite, just run from your terminal:

```shell
$ [sudo] apt install sqlite3
```

## Install from Source

You can also download the source code [here](https://sqlite.org/download.html) and build from scratch. After you have the source code in your local folder, run the following commands in your terminal.

```shell
$ tar -xvf sqlite-autoconf-3310100.tar.gz
$ cd sqlite-autoconf-3310100/
$ ./configure --prefix /usr/local/
$ make
$ make install
```

## Test

To test if you have installed SQLite on your machine correctly, you can run `sqlite3` in your terminal:

```shell
$ sqlite3
SQLite version 3.22.0 2018-01-22 18:45:57
Enter ".help" for usage hints.
Connected to a transient in-memory database.
Use ".open FILENAME" to reopen on a persistent database.
sqlite> 
```

