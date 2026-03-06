---
Category: 1
---
# OwnCDN origin story

We (JH Software) also develop and run an educational platform with on-line tests and exercises for Danish elementary and middle schools - see https://tjek.net (Danish language only).

For years, we ran this as a single ASP.NET website under IIS on a Windows VPS (virtual private server) at various cloud providers.
But when GDPR (EU privacy regulations) hit, it became difficult to be in compliance while keeping the data with cloud providers.

So, we decided to move the core of Tjek.net home to a server running in our own office where we can ensure privacy and security for our users in accordance with GDPR.

As part of Tjek.net, we also serve a lot of images and videos (not user-specific) as illustrations in the on-line tests and exercises, and we didn't want to serve these through the limited bandwidth of our office Internet connection.

Since we were still running a (now underutilized) Windows VPS at a cloud provider for other purposes, we wanted to try and use this for serving the images/videos and to cache some dynamically generated content from the office server.

This meant that we needed some kind of object storage software (like AWS S3) and web caching software (like a CDN) running on this server.

Since we couldn't find any suitable software for this, we started putting together our own.

After refining this software for several years, this is, of course, what eventually became OwnCDN.

Today OwnCDN is serving 250K+ images/videos for Tjek.net every day, while barely registering on the CPU usage chart on the VPS.
