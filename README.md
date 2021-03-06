# proxify
Generate nginx &amp; dnsmasq configuration, plus .passwd, ssl certificates, &amp; cloudflare/dnsimple shell scripts for your reverse proxy

```
Usage: proxify (<hostname> | <file>) [:listen] [:target] [--options]...

Options:
  -d, --DOMAIN        Domain name sub-domains built on                   [default: "local"]
  -i, --SERVER        Private IP address of the host server          [default: "127.0.0.1"]
  -t, --ROUTER        Domain pointing to home router              [default: "router.local"]
  -o, --OUTPUT        Output directory, used in configuration             [default: "/etc"]
  -u, --USER          User account running process                    [default: "www-data"]
  -c, --CA            Certificate Authority URL         [default: "http://127.0.0.1:11443"]
  -p, --PASSWORDS     Comma-delimited name:password          [default: "www-data:www-data"]
  -l, --CLOUDFLARE    email:key
  -n, --DNSIMPLE      email:key
  -x, --nginx         Additional nginx configuration                       [default: false]
  -s, --secure        Create secure host & certificate                     [default: false]
  -a, --authenticate  Authenticate username or certificate                 [default: false]
  -r, --redirect      Redirect to target                                          [boolean]
  -f, --force         Force overwriting files                                     [boolean]
  -h, --help          Show help                                                   [boolean]

```

## Installation  

`npm install -g suderman/proxify`  
