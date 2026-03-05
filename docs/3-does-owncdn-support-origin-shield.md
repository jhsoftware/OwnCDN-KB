---
category: 1
---
# Does OwnCDN support "Origin Shield"

Yes.

"Origin Shield" is a term used when a CDN service uses a single caching node to forward requests (for URLs not yet cached) to the origin server, on behalf of all other caching nodes of the CDN service.

If the CDN service has many caching nodes (typically distributed around the world), having each of these forward requests directly to the origin server could potentially increase the traffic to the origin server by a factor equal to the number of caching nodes of the service.

You can do the same with OwnCDN.

Set up one OwnCDN server to fetch from the origin server and configure any additional OwnCDN servers to fetch from the first OwnCDN server.


