tgcd-windows
============

Description
-----------
The great `TCP Gender Changer (tgcd)` compiled for Windows.  


Features
--------
* Latest `v1.1.1` version
* Compiled for `x86` so should work on `x86` and `x64` platforms (tested on Win XP and 10)
 

Usage
-----
1. `git clone` the repo or download the [whole archive](https://github.com/maaaaz/tgcd-windows/archive/master.zip)
2. Extract it and run it
3. Profit


Options
-------
```
> tgcd.exe
TCP Gender Changer, V1.1.1 Copyright (C) 2016 Faraz.V (faraz@fzv.ca)
Usage: tgcd { -C | -L | -F }  options ...

Options are:

 ConnectConnect mode: tgcd -C -s host:port -c host:port [-i n ] [-k n ] [ common options ]
 ConnectConnect :
 -C, --ccnode               Become a CC (ConnectConnect) node.
 -s, --server host:port     The host and port of the actual server
 -c, --llhost host:port     The host and port of the ListenListen node.
 -i, --interval seconds     Time interval to periodically report to LL (default: 40s).
 -k, --key number           Poorman's encryption (0-255, default: 0, means no encryption)

 ListenListen mode: tgcd -L -p port  -q port  [-k n ] [ common options ...]
 -L, --llnode               Become a LL (ListenListen) node.
 -q, --llport number        The port to listen on for incomming connection from a CC node
 -p, --port number          The port to listen on for incomming actual client connection
 -e, --interface            The interface for incomming actual client connection (default: all interfaces)
 -k, --key number           Poorman's encryption (0-255, default: 0, means no encryption)

 PortForwarder mode: tgcd -F -p port -s host:port [ common options ... ]
 -F, --lcnode               Become a ListenConnect node, i.e. just a simple port forwarder
 -p, --port  number         The port to listen on for incomming actual client connection
 -s, --server host:port     The host and port of the actual server or a LL node

Common options:
 -m, --method { f | s }     f: Fork  s: Select (default: s)
 -f, --filter filter        Optional argument to run a filter on new connections, IP passed as argument
 -l, --log file             Write logs to file. (default:'')
 -g, --level number         Log level detail (default:0).
 -n, --nodaemon             Do not become daemon
 -h, --help                 Display this.
 -v, --version              Display version number.
```

Older versions
--------------
* Browse the [release section](https://github.com/maaaaz/tgcd-windows/releases) to find some old versions


Disclaimer & licence 
---------------------
* This software is provided under the original [tgcd's licence](http://tgcd.sourceforge.net/#lbAI)
* Do not use it for illegal purposes
* I don't own anything on the tgcd brand and am not affiliated with this project
* Last but not least, antivirus softwares might report some binaries as hacktools or even malwares: this is a known and common issue. If you don't trust this compilation: 
  1. Just don't download it.
  2. Compile it yourself


Credits
-------
* Faraz V for its cool [tool](http://tgcd.sourceforge.net)