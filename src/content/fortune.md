Title: Fortune Web Service
Author: Andrew Boring
Date: 2019-09-17
Slug: fortune
Category: projects

[Fortune](http://fortune.a10g.com) is a public web service serving fortunes via simple REST API.  


The web service is available at http://fortune.a10g.com.  
Source code is available at https://github.com/a10g/qsrv.

## Project Summary
Fortune is a web service in the tradition of the Unix fortune(6) program. It serves random fortunes assembled from traditional Unix/Linux fortune files and new collections assembled by the project. Fortune aims to be the definitive source for quotes, fortunes, one-liners, and tips-n-tricks on-demand.


## Project Details
The original objective behind this project was tos advance a personal effort by the project's maintainer to popularize a collection of quotes by The Mighty Monarch, a character from the Adult Swim animated series, The Venture Bros.

This collection of quotes was organized into the [fortune file format](https://en.wikipedia.org/wiki/Fortune_(Unix)#Fortune_files), ultimately intended to be included into various OS distributions that provide the program and a collection of fortune files.

The effort was misguided: no one uses fortune(6) anymore.

The FreeBSD project [removed their fortune files](https://svnweb.freebsd.org/base?view=revision&revision=325828) in 2017 (though it has since moved to Ports), and macOS no longer distributes fortune with their BSD userland either. Most Linux distributions don't install it by default, and Windows never had it to begin with. People these days prefer laptops over workstations, mobile devices over laptops, and the whole notion of a "login" has changed so radically that there is simply no room for a fortune program in today's modern computing environment.

Or is there?

In this larger, more _complex_ computing world, web services power web applications that power social media sites and personal blogs and line-of-business applications and all sorts of stuff. This is becoming infrastructure. A _logical_ (eg, not physical) infrastructure, but infrastructure nonetheless.

Unix evolves. We may not have the Unix Version 7 anymore, but we have macOS; we have the BSDs keeping the Berkeley legacy alive; and we have more Linux distributions than are digits in Pi. All of these have some cultural legacy, but still need to change with the times and the need. Those that have no evolutionary path, cease to exist.

This web service is an attempt to provide that evolutionary path to a simple Unix utility whose contents brought simple joy to so many people through the years. Perhaps it can continue to provide it for years to come.


## Terms:

- This web service is free to use.
- Currently, there are no rate limits or other restrictions. As this service gains usage, reasonable  restrictions may be put in place to prevent service issues. Any application developers looking to use this service in their application are absolutely welcome to, with the notice that no service level is being provided. As-is.
- Any businesses, organizations, or app developers requiring a service level agreement are welcome to contact me for options.

## Usage:

```
/api
Returns API information and usage.
(not yet implemented)
```
```
/api/fortune/list
List all fortune files.
```
```
/api/fortune/random
Returns a random fortune from all available fortune file.
```
```
/api/fortune/{database}
Returns a fortune from the selected fortune file.
```
