---
title: CarOS 15.12 Basketane
layout: post
---


~~~
    
   ______           ____  _____    /\
  / ____/___ ______/ __ \/ ___/   /  +---+
 / /   / __ `/ ___/ / / /\__ \    \  |  /|  CarOS 15.12
/ /___/ /_/ / /  / /_/ /___/ /     +---+ +  Basketane
\____/\__,_/_/   \____//____/      |   |/   http://caros.io/
                                   +---+

~~~

### Features


* security fixes from poky-upstream (1.8.1)
* added tools required for virtualization
* basic support for host-based firewall (native tools + rule persistence)
* preliminary support for self-hosted package feeds (added "kellner")
* added openvswitch
* added unbound and nsd packages for DNS resolving and zone-serving
* added nginx-1.9.6

For more details see [changelog][4]

### Why basketane? 
 
"Basketane is a polycyclic alkane with the chemical
formula C10H12. The name is taken from its structural similarity to a basket
shape." see [wikipedia][1]
 
Caros 15.12 supports KVM, it's like a basket.
 
<!-- more -->
Well, what should we add to the basket? How can we show it works? What could
we do next? What do you need?
 
First Patch: Caros itself. We will add a little HowTo about setting up self hosted package
feeds.
 
Second Patch: little tiny KVMs, i.e. unit tests like
[KVM-unit-tests][2].
It is a kind of positive egoism. To show it works and alert ourself when it's
broken.

Btw. CarOS is a rolling release - we drop a new release every 16th of a month.
You can download an ISO-, OVA- or sdcard-image for [**CarOS - release 15.12**][3] or set up your own buildroot using the [REDOMAT][5] definition

[1]: https://en.wikipedia.org/wiki/Basketane
[2]: http://www.linux-kvm.org/page/KVM-unit-tests
[3]: https://github.com/carosio/caros-release/releases/tag/v15.12 
[4]: https://github.com/carosio/caros-release/blob/master/CHANGELOG.md
[5]: https://github.com/carosio/redomat
