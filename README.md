<!--<h1 align="center">
  <br>
  <a href="http://github.com/fonoster/routr"><img src="https://raw.githubusercontent.com/wiki/fonoster/routr/images/logo.png" alt="Running Routr" width="150"></a>
  <br>
  Routr
  <br>
</h1>-->

<h2 align="left">Next-generation Sip Server.</h4>

<p align="left">
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg"
         alt="License: MIT">
  </a>
</p>

<p align="left">
  <a href="#key-features">Key Features</a> •
  <a href="#quick-start">Quick Start</a> •
  <a href="#bugs-and-feedback">Bugs and Feedback</a> •
  <a href="#Contributing">Contributing</a> •
  <a href="#license">License</a>
</p>

## Key Features

- Proxy
- Registrar Service
- Location Service
- Call Forking
- Multi-Tenancy/Multi-Domain
- Access to the PSTN Using SIP Gateways
- Transport: TCP, UDP, TLS, WebSocket
- Data Sources: Redis, Restful API, Files
- Restful API
- Command Line Tool for Admin Operations
- Routing Capabilities
  - Intra-Domain Routing (IDR)
  - Domain Ingress Routing(DIR)
  - Domain Egress Routing (DER)
  - Peer Egress Routing (PER)
- Security
  - Digest SIP User Authentication
  - Domain Access Control List (DACL)
  - Restful service secured with TLS and JWT tokens

To learn more, read the [documentation](https://fonoster.github.io/routr). :books:

## Quick Start

**Download the server**

| Platform | Download |
| -- | -- |
| Linux | [tar.gz](https://github.com/fonoster/routr/releases/download/1.0.0-rc1/routr-1.0.0-rc1_linux-x64_bin.tar.gz) |  
| macOS | [tar.gz](https://github.com/fonoster/routr/releases/download/1.0.0-rc1/routr-1.0.0-rc1_osx-x64_bin.tar.gz) |  
| Windows | [tar.gz](https://github.com/fonoster/routr/releases/download/1.0.0-rc1/routr-1.0.0-rc1_windows-x64_bin.tar.gz), [zip](https://github.com/fonoster/routr/releases/download/1.0.0-rc1/routr-1.0.0-rc1_windows-x64_bin.zip) |  
| Docker | [img](https://hub.docker.com/r/fonoster/routr/) |  

**Running with Docker**

```bash
docker pull fonoster/routr
docker run -it \
    -p 4567:4567 \
    -p 5060:5060 \
    -p 5060:5060/udp \
    -p 5061-5063:5061-5063 \
    -e ROUTR_EXTERN_ADDR=${your host address} \
    fonoster/routr
```
**Running with any other platform**

```bash
cd routr.1.0.0-rc1
./routr
```

## Bugs and Feedback

For bugs, questions, and discussions please use the [Github Issues](https://github.com/fonoster/routr/issues)

## Contributing

For contributing, please see the following links:

 - [Contribution Documents](https://github.com/fonoster/routr/blob/master/CONTRIBUTING.md)
 - [Contributors](https://github.com/fonoster/routr/contributors)

## Authors
 - [Pedro Sanders](https://github.com/psanders)

## LICENSE
Copyright (C) 2018 by [Fonoster Inc](https://github.com/fonoster). MIT License (see [LICENSE](https://github.com/fonoster/routr/blob/master/LICENSE) for details).
