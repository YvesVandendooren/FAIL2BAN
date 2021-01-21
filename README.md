# Ansible role `Fail2ban`

Ansible role for basic setup of fail2ban on CentOS 8

## Requirements

No specific requirements


## Role Variables

Nono of the variables are required. If you don't define them, the default values in [default values](defaults/main.yml) will be used

### Basic configuration

| Variable                       | Default         | Comments                                                                                                     |
| :---                           | :---            | :---                                                                                                         |
| `fail2ban_ignoreip`         | 127.0.0.1/8     | This is a list of IP addresses, CIDR masks or DNS hosts, Fail2ban will not ban   |
| `fail2ban_bantime` | 10m           | This is the number of seconds a hosts will be banned for|
| `fail2ban_findtime`           | 10m              | A host is banned if it has generated `maxretry` during the last `findtime`|
| `fail2ban_maxretry`            | 5              | This is the number of failures before a host gets banned|