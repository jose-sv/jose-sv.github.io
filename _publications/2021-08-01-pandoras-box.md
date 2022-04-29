---
title: "Opening Pandora’s Box: A Systematic Study of New Ways Microarchitecture Can Leak Private Data"
collection: publications
permalink: /publication/pandoras_box
excerpt: 'Our study uncovers seven classes of microarchitectural optimization with novel security implications, proposes a conceptual framework through which to study them and demonstrates several proofs-of-concept to show their efficacy. The optimizations we study range from those that leak as much privacy as Spectre/Meltdown (but without exploiting speculative execution) to those that otherwise undermine security-critical programs in a variety of ways.'
date: 2021-08-01
venue: 'ISCA'
paperurl: 'https://ieeexplore.ieee.org/document/9499823'
citation: '<a href="#bibtex-pandora" class="open-popup-link">bibtex</a> | <a href="#nontex-pandora" class="open-popup-link">Plain Text</a>'
---
{% include citations.html %}

Microarchitectural attacks have plunged Computer Architecture into a security crisis. Yet, as the slowing of Moore’s law justifies the use of ever more exotic microarchitecture, it is likely we have only seen the tip of the iceberg.To better anticipate this security crisis, this paper performs a systematic security-centric analysis of the Computer Architecture literature. Our rationale is that when implementing current and future processors, microarchitects will (quite reasonably) look to previously-proposed ideas. Our study uncovers seven classes of microarchitectural optimization with novel security implications, proposes a conceptual framework through which to study them and demonstrates several proofs-of-concept to show their efficacy. The optimizations we study range from those that leak as much privacy as Spectre/Meltdown (but without exploiting speculative execution) to those that otherwise undermine security-critical programs in a variety of ways. Many have storied histories— ranging from industry patents to media/3rd party speculation regarding current implementation status to recent renewed interest in the academic community. This paper’s goal is to perform an early (hopefully not too late) analysis to inform their development moving forward.
