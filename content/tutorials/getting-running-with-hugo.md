---
title: "Getting Running With Hugo"
date: 2020-07-22T22:15:53Z
draft: true
---



**n.b.** Plenty of great resources are avilable and I used a mixture of the offical [getting started](https://gohugo.io/getting-started/quick-start/) guide and some pointers for the appropriate container. 

It is worth noting that I don't like installing devkits or tools directly on my laptop. Why you ask well invariably doing starts the clock tiking on when I need to completely purge the machine. No this means I have a few options open to me:
- VM - I could install everything on a VM and simply wipe that later when done, but I'm not a fan of doing that either it's a little irrational but I used to have to work in theat environment over 10 years ago and the performance issues I faced, well enough said. Further to that I really hate the idea of maintaing and patching another image. 
- Cloud VM - Now I love the cloud and this is a possible option but I like the idea that I can work especially on development without my connection having to be rock solid. Remoting to a machine in another data center mean that any issue with my connectivity and I lose productivity. 
- Container - Now this is my personal choice, a container is started based on an image that I coudl create or just use one someone else has used. The overhead of virtualisation doesn't come into play as it shares the kernal with the host. And they don't take up loads of space.
