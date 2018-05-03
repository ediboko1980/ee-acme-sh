# ee-acme-sh

### Bash script to install Let's Encrypt SSL certificates automatically using acme.sh on servers running with EasyEngine

![ee-acme-sh](https://raw.githubusercontent.com/VirtuBox/ee-acme-sh/master/ee-acme.png)

## Features

-   Automated Installation of Let's Encrypt SSL certificates using [acme.sh](http://acme.sh)
-   Acme validation with standalone mode or Cloudflare DNS API
-   Domain, Subdomain & Wildcard SSL Certificates support
-   IPv6 Support
-   ECDSA Certificates with ECC 384 Bits private key
-   Automated Certificates Renewal


## Installation

```bash
cd && bash <(wget --no-check-certificate -O - https://raw.githubusercontent.com/VirtuBox/ee-acme-sh/master/install.sh)

# enable acme.sh & ee-acme-sh
source .bashrc
```

## Usage :

```bash
# Install a SSL certificate on a domain + alias www
ee-acme-www

# Install a SSL certificate on a subdomain 
ee-acme-subdomain 

# Install a Wildcard SSL certificate on a domain 
ee-acme-wildcard 
```

## Limitations

-   Wildcard certs are only available with Cloudflare DNS API 
 
