# SQLite Install Guide

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

To test if you have installed SQLite on your machine successfully, you can run `sqlite3` in your terminal:

```shell
$ sqlite3
SQLite version 3.22.0 2018-01-22 18:45:57
Enter ".help" for usage hints.
Connected to a transient in-memory database.
Use ".open FILENAME" to reopen on a persistent database.
sqlite> 
```

If you saw the above prompt, the installation is completed.

# SQLite 安装文档

这篇文档将指引你在Ubuntu 18.04 LTS x64上安装SQLite。

## 通过 `apt` 安装

你可以在终端中利用如下命令安装SQLite：

```shell
$ [sudo] apt install sqlite3
```

## 通过源码安装

你也可以在[这里](https://sqlite.org/download.html)下载源码并通过源码安装，如果源码已经下载到本地，可以在终端中输入如下命令：

```shell
$ tar -xvf sqlite-autoconf-3310100.tar.gz
$ cd sqlite-autoconf-3310100/
$ ./configure --prefix /usr/local/
$ make
$ make install
```

## 测试

若要测试SQLite是否成功安装，在命令行中运行：

```shell
$ sqlite3
SQLite version 3.22.0 2018-01-22 18:45:57
Enter ".help" for usage hints.
Connected to a transient in-memory database.
Use ".open FILENAME" to reopen on a persistent database.
sqlite> 
```

出现以上提示后，则表明安装成功。