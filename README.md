# set-proxy-to-terminal

set proxy to terminal (bash and zsh) (http - https - socks5)

## Set Up

Installation prerequisites :

-   jq : Download jq and install (https://stedolan.github.io/jq/download/)
-   Tor Browser (optional) (https://www.torproject.org/download/)
-   tor (optional) (https://gist.github.com/lukechilds/0be1d56ecd28092822e4fa750b5945c0)

add code :

```zsh
source $HOME/[Directory]/setProxy
```

to `.zshrc` or `.bashrc`

---

## help

```text
$ setProxy -h
 --------------------
 $ setProxy [option]

 [option]
    -t | tor                   : set proxy default tor port 9050
    -t2 | tor2                 : set proxy default tor port 9150
    -s [Proxy] | set [Proxy]   : set Proxy custom
    -me | me                   : set proxy default config me (socks5://127.0.0.1:1089)
    -d | --unset | d | unset   : un set Proxy in terminal
    -h | --help | help         : echo Help
    -status | status           : echo Status
    -err                       : echo show Errors

 [Proxy]
    -P [Protcol]               : set Protcol (h = http, hs = https, s5 = socks5) (default s5)
    -H [Host] | Host [Host]    : set Host Proxy custom (default 127.1)
    -p | prot                  : set port Proxy custom (default 9050)

 [Host]
    -H [HostName]              : set Host (127.1, 127.0.0.1 , ::, Hsot external{Domain})

 [example]
    -> example: http://127.0.0.1:1089
    -> example: -s -P h -H 127.1 -p 1089

    -> example: https://127.0.0.1:8889
    -> example: set -P hs -H 127.1 -p 8889

    -> example: socks5://127.0.0.1:9050
    -> example: set -P s5 -H 127.1 -p 9050

 myExample: $ setProxy socks5://127.1:9050
 myExample: $ setProxy set -P s5 -p 9050
 myExample: $ setProxy set -P s5 -H 127.1 -p 9050
 myExample: $ setProxy set -H 0
 myExample: $ setProxy me

```

<!-- photos  -->
<!-- ![$ setProxy tor](https://) -->

[my page](http://rm1378.me/)
