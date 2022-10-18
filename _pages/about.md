---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

Hello! I am a Hardware Security Researcher at Intel's Security Assurance and Cryptography group.

My Ph.D. advisor was [Chris Fletcher](http://cwfletcher.net/) at at the University of Illinois at Urbana-Champaign.
My graduate research performed the first broad, systematic study of the microarchitecture literature to characterize the security implications of both known and new (theorized) microarchitectural optimizations [[1]](https://jose-sv.github.io/publication/pandoras_box).
To facilitate this study, we developed a novel abstraction to precisely and concisely capture potential leakage while abstracting away the victim program and threat model.
This study discovered, for the first time, that microarchitecture outside of speculative instruction execution is capable of forming a "universal read gadget" (URG).
A variant of this microarchitecture was subsequently discovered in Apple silicon, which proved to be the first microarchitecture (in the wild) capable of leaking data at rest [[2]](https://jose-sv.github.io/publication/augury).

You can learn more about this second work, Augury, at [prefetchers.info](https://www.prefetchers.info/)!
Here's a [twitter thread](https://twitter.com/dkohlbre/status/1520080542221631489) about it too.
Our experiments demonstrate the existence of a pointer-chasing DMP on recent Apple processors, including the A14 and M1.
We then reverse engineer the details of this DMP to determine the opportunities for and restrictions it places on attackers using it.
Finally, we demonstrate several basic attack primitives capable of leaking pointer values using the DMP.

I received my B.S. from Lawrence Technological University (in Southfield, MI),
where I was a two time recipient of a Presidential Research Grant.
I went on to complete my M.S. at the University of Illinois at Urbana-Champaign
in the fall of 2019.
My M.S. culminated in the introduction of
[Asynchronous Poisoning Attacks](https://jose-sv.github.io/publication/2020-03-01-game-of-threads).

 Feel free to contact me josers2 [at] illinois [dot] edu with any questions
 about my papers, research, or anything else.
