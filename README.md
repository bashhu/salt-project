# salt-project
#salt的sls通用工程
- base : system init ,software install
- prod : server config and start shell
.
├── base
│   ├── haproxy
│   │   ├── files
│   │   │   ├── haproxy-1.6.10.tar.gz
│   │   │   └── haproxy-init
│   │   └── install.sls
│   ├── init
│   │   ├── files
│   │   │   ├── limits.conf
│   │   │   └── resolv.conf
│   │   ├── pkg.sls
│   │   ├── resolv.sls
│   │   ├── rsyslog.sls
│   │   ├── sysctl.sls
│   │   └── www.sls
│   ├── keepalived
│   │   ├── files
│   │   │   ├── keepalived-1.3.1.tar.gz
│   │   │   └── keepalived-sysconfig
│   │   └── install.sls
│   ├── nginx
│   │   ├── files
│   │   │   ├── nginx-1.10.2.tar.gz
│   │   │   └── pcre-8.38.tar.gz
│   │   └── install.sls
│   └── top.sls
├── prod
│   ├── cluster1
│   │   ├── files
│   │   │   ├── blog.nginxs.net.conf
│   │   │   ├── haproxy.cfg
│   │   │   ├── haproxy-init
│   │   │   ├── keepalived.conf
│   │   │   ├── keepalived-init
│   │   │   ├── keepalived.service
│   │   │   ├── nginx.conf
│   │   │   └── nginx-init
│   │   ├── haproxy_keepalived.sls
│   │   └── nginx.sls
│   └── top.sls
└── README.md
