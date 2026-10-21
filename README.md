# Web Infrastructure Design

This project covers the design of web infrastructures, from a single-server LAMP-style stack up to a scaled, secured and monitored multi-server architecture. Each task is a whiteboard exercise: design the infrastructure, take a picture of the diagram, and be able to explain every component and its weaknesses.

## Concepts

- Network basics
- Server
- Web server
- DNS
- Load balancer
- Monitoring

## Acronyms

| Acronym | Meaning |
|---------|---------|
| LAMP | Linux, Apache, MySQL, PHP (here Nginx replaces Apache) |
| SPOF | Single Point of Failure |
| QPS | Queries Per Second |

## Tasks

| # | File | Description |
|---|------|-------------|
| 0 | [0-simple_web_stack](./0-simple_web_stack) | One server hosting `www.foobar.com` (Nginx, application server, code base, MySQL) |
| 1 | [1-distributed_web_infrastructure](./1-distributed_web_infrastructure) | Three servers: HAProxy load balancer plus two servers, MySQL Primary-Replica |
| 2 | [2-secured_and_monitored_web_infrastructure](./2-secured_and_monitored_web_infrastructure) | Adds 3 firewalls, an SSL certificate for HTTPS, and 3 monitoring clients |
| 3 | [3-scale_up](./3-scale_up) | Adds a second load balancer (cluster) and splits web, application and database onto their own servers |

## Notes

- Each answer file starts with the link to the screenshot of the whiteboard diagram.
- Everything is written in English.
- Each diagram is whiteboarded in front of a reviewer without notes, within 30 minutes, covering only what the requirements ask.
