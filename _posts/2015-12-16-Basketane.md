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

* (support for KVM virtualized guests)
* basic support for host based firewall (native tools + rule persistence)
* preliminary support for package feeds (self-hosted too with "kellner")
* openvswitch
* (quagga/ISIS)

### Why basketane? 
 
"Basketane is a polycyclic alkane with the chemical
formula C10H12. The name is taken from its structural similarity to a basket
shape." see [wikipedia][1]
 
Caros 15.12 supports KVM, it's like a basket.
 
<!-- more -->
Well, what should we add to the basket? How can we show it works? What could
we do next? What do you need?
 
First Patch: Caros itself, we add a little HowTo for setup a self hosted package
feeds to our Caros.io webpage.
 
Second Patch: little tiny KVMs, i.e. unit tests like
[KVM-unit-tests][2].
It is a kind of positive egoism. To show it works and alert ourself when it's
broken.


[1]: https://en.wikipedia.org/wiki/Basketane
[2]: http://www.linux-kvm.org/page/KVM-unit-tests.
