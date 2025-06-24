---
title: DNS
nav_order: 5
---
# DNS
Api versioning should be added, if non provided it should default to v1.

## Versions
- [v2](v2.md)

## Domain names
Each segment of a domain name needs to follow the following regex:\
`/^[a-z0-9\-]{1,24}$/mi`\
Full length regex:
`/^([a-z0-9\-]{1,24}\.)+[a-z0-9\-]{1,24}$/mi`