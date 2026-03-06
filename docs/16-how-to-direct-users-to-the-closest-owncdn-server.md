---
Category: 4
---
# How to direct users to the closest OwnCDN server

Having content caching servers geographically closer to users means reduced network latency, and thus faster content delivery.
Setting up multiple CDN "exit nodes" around the world is a common method used to achieve this.

You can, of course, also do this with OwnCDN.

There are a couple of methods of routing traffic to the caching server closest to each user:

## Anycast

[Anycast](https://en.wikipedia.org/wiki/Anycast) is a method where one IP address can actually represent different endpoints, depending on geographical location, controlled by IP routing tables.

This is generally only available to large ISPs and global network operators. Contact your Internet provider for more information on this.   

## GeoDNS

GeoDNS is where the DNS servers for your domain name point to different IP addresses depending on where the DNS request originates from.

This is not a standard DNS feature, but is offered by some DNS service providers and available in some DNS server software packages.

For example, there is a [GeoDNS plug-in](https://simpledns.plus/kb/177-geodns-plug-in) available for [Simple DNS Plus](https://simpledns.plus).

