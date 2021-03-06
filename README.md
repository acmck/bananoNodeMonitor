# Banano Node Monitor

![GitHub release](https://img.shields.io/github/release/nanotools/nanoNodeMonitor.svg?style=flat-square) [![StyleCI](https://styleci.io/repos/118352667/shield?branch=master)](https://styleci.io/repos/118352667)

Banano Node Monitor is a server-side PHP-based monitor for a Banano node. It connects to a running node via RPC and displays it's status on a simple webpage. Being server-side, it does not expose the RPC interface of the Banano node to the public. 

![Desktop screenshot](https://i.imgur.com/tuecnSK.png)


## Prerequisites

- Running Banano Node with RPC enabled ([Tutorial](https://github.com/nanocurrency/raiblocks/wiki/Docker-node))
- Webserver with PHP ([Tutorial](https://www.digitalocean.com/community/tutorials/how-to-install-linux-nginx-mysql-php-lemp-stack-in-ubuntu-16-04))
- PHP-Curl Module

    `sudo apt-get install php-curl`

## Installation

In your empty webserver directory, e.g. `/var/www/html`, execute:

    git clone https://github.com/BananoTools/bananoNodeMonitor .

 
If you want it to run a subdirectory remove the `.` at the end.

In the `modules` folder, create your own config file by executing:


    cp config.sample.php config.php


If you run a standalone node you might need to modify the IP-address and the port for the RPC in the file `config.php`. It should match the corresponding entries in `~/Banano/config.json`, e.g.

```
// ip address for RPC (default: [::1])
$nanoNodeRPCIP   = '127.0.0.1';

// ip address for RPC (default: 7076)
$nanoNodeRPCPort = '7072';
```

## Updating
Switch to your installation directory and execute `git pull`.

## Links

* [Banano Repo](https://github.com/BananoCoin/banano)


## Support

Feel free to change your representative to my Banano node `ban_3w3k96jibqym7c9cer7web88tbk9uzabx9jtq9iphhwkkqdpnywe8e1gset7` to support further decentralization within the Banano network. In case of problems, please send an [issue](https://github.com/BananoTools/bananoNodeMonitor/issues). 

Donations are welcome to: [ban_3w3k96jibqym7c9cer7web88tbk9uzabx9jtq9iphhwkkqdpnywe8e1gset7](https://www.nanode.co/account/xrb_1f56swb9qtpy3yoxiscq9799nerek153w43yjc9atoaeg3e91cc9zfr89ehj)

Have fun! :)





