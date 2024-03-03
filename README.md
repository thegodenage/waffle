# WAFFLE

## Introduction
Probably you know about CloudFlare, every one knows, but this is a partially paid solution. As the open source community
we are missing a real modular and open source **Web Application Firewall** that could be used in the place of CF.

## How to run / Develop ?

### Prerequisites 
+ Go 1.22
+ make (if windows, try using chocolatey)
+ openssl (if windows, try using git bash)

1. Create certificates and FS embed go file provider `make certs_windows`
2. Execute `docker compose up -d` to create needed infrastructure
3. Set environment variables before running the proxy:
```
DATABASE_URI=dns:passpass@tcp(localhost:3306)/dns
```

### Generate certificates
Execute make certs_windows and go through process. It should certs in the .cert directory.

## Planned features / Architecture
To bo honest, I'm learning how to write WAF from the scratch, so this part will be updated after a while. 

## Education
[A Comprehensive Examination of Cloudflare's IP-based Distributed Denial of Service Mitigation](https://www.researchgate.net/publication/375238537_A_Comprehensive_Examination_of_Cloudflare%27s_IP-based_Distributed_Denial_of_Service_Mitigation)