# Hypernode SSH Brancher
Simple SSH script to connect to your active branchers.

Where you normally type `ssh -l app yourhypernode.hypernode.io` replace it with `ssh-brancher -l app yourhypernode.hypernode.io`

## Supported SSH options
We've builtin support for the following ssh options
- `-l`: Login name (most probably `app`)
- `-i`: SSH key to use
- `-p`: Alternative port number

## Installation
Download [ssh-brancher](https://raw.githubusercontent.com/elgentos/hypernode-ssh-brancher/main/ssh-brancher) to a bin directory and give it execution permissions.

## Usage

```
# usage
$ ssh-brancher
Usage ssh-brancher (options) [HOST] ...args

# login
$ ssh-brancher -l app yourhypernode.hypernode.io
1: yourhypernode-ephnmf3ai.hypernode.io
Which brancher do you want to connect to? [0 to exit, default 1]

# ...
  /\  /\_   _ _ __   ___ _ __ _ __   ___   __| | ___
 / /_/ / | | | '_ \ / _ \ '__| '_ \ / _ \ / _` |/ _ \
/ __  /| |_| | |_) |  __/ |  | | | | (_) | (_| |  __/
\/ /_/  \__, | .__/ \___|_|  |_| |_|\___/ \__,_|\___|
        |___/|_|

# ...

app@yourhypernode-ephnmf3ai.hypernode.io:~$ 
app@yourhypernode-ephnmf3ai.hypernode.io:~$  exit

# direclty execute command
$ ssh-brancher -l app yourhypernode.hypernode.io 'hypernode-systemctl settings'
1: yourhypernode-ephnmf3ai.hypernode.io
Which brancher do you want to connect to? [0 to exit, default 1]

usage: hypernode-systemctl settings php_version 7.1                                                      
                                                                                                         
The possible values are:                                                                                 
# ....

$

```

## Authors
- [Jeroen Boersma](https://github.com/JeroenBoersma)
- [elgentos](https://elgentos.nl/)

