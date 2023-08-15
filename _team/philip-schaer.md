---
name: "Philip Schär"
role: "PhD student"
ordering: 3
imgpath: "/assets/Philip_preliminary.png"
teaser: "Researches slice sampling"
layout: member
---

I am a second-year PhD student in mathematics, working on slice sampling under joint supervision of [Michael Habeck](/team/michael-habeck.html) and [Daniel Rudolf](https://staff.fim.uni-passau.de/~rudolf/).  

Slice sampling is a class of Markov chain Monte Carlo (MCMC) methods for approximate sampling from (absolutely continuous) probability distributions on (potentially high-dimensional) Euclidean spaces. It can generally be divided into two-subclasses, *ideal slice sampling* and *pragmatic slice sampling*. Methods in the former are conceptually simple and correspondingly well-analyzable, but parts of their transition mechanism cannot be efficiently implemented (except in some toy settings), which prevents them from being used in practical applications. Pragmatic slice sampling methods on the other hand are specifically designed to be efficiently implementable, while each mimicking a specific ideal slice sampler in hopes of retaining some of its properties, and have found good use in a variety of practical applications. However, the commitment to computational efficiency has so far only led to methods that are conceptually quite complicated (at least compared to their ideal slice sampling counterparts) and correspondingly hard to formally analyze.

My PhD project concerns itself both with ideal and with pragmatic slice sampling methods. On the one hand, we aim to further improve the theoretical understanding of ideal slice sampling methods, for example by deriving better estimates of their spectral gap, which is known to quantify both the convergence speed and the asymptotic sample quality of an MCMC method for a given target distribution. In our view, results in this regard serve both to underline advantages of slice sampling over other MCMC approaches and to point out performance disparities between different ideal slice samplers.

On the other hand, we are interested in the development of new pragmatic slice sampling methods. By mimicking previously underexplored ideal slice samplers (such as *polar slice sampling*), we hope to devise new MCMC methods that, at least in certain types of settings, outperform all existing ones. This in turn necessitates some theoretical work, because for pragmatic slice samplers merely proving their asymptotic convergence already poses a significant challenge.


## My Pages

[arXiv Publications](https://arxiv.org/a/schar_p_1.html)  
[Google Scholar](https://scholar.google.com/citations?hl=en&user=tIE_vOQAAAAJ)  
[Research Gate](https://www.researchgate.net/profile/Philip-Schaer)  
[Semantic Scholar](https://www.semanticscholar.org/author/Philip-Schar/2204760249)  
[LinkedIn](https://www.linkedin.com/in/philip-sch%C3%A4r-6a190b250)

## Publications
{% include publication-list.html name="philip" %}

