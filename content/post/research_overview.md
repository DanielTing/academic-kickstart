---
title: "Research overview"
date: 2019-09-20T08:47:11+01:00
draft: false
---

As with any researcher, I’m often asked what my research area is. Mine is Data Sketching. It can be considered a somewhat niche area, but it's one I’m quite excited about. It can have incredible impact in how people use data, and imho is a beautiful marriage of statistical theory and a practical problem. Fundamentally, it boils down to solving the following question:

In the world of massive datasets, is it possible to remove the main barrier that makes processing Big Data slow: namely, the bigness of the data? 

That may seem like a silly question. After all, why would Big Data be revolutionary except for the fact that it's BIG. But consider what statisticians have done for decades, constructing small datasets (samples) from a much larger population to answer questions using data with confidence. All that matters is ensuring the information content of the dataset is sufficient for answering the questions at hand. 

Data sketches do just that. They preserve the relevant information in a small amount of space. Furthermore, they provide the necessary assurance that the answers can be trusted, with hard theoretical guarantees even against adversarial data. 

The space savings can be huge. For example, a common ad metrics reporting problem is to count the distinct impressions for an ad. One sketch, HLL, can count this in just 5kB of space, at roughly 1% accuracy. Compare that to constructing a hash table for a site with up to 1B users. That can easily take 8GB or over 1 million times more space!

While this is awesome, sketches have some crucial limitations. In particular, a single data sketch answers a limited set of questions. It throws away the data on “unimportant” questions to achieve its space savings. These questions depend both on the type of sketch and the parameters chosen. This leads to some vexing choices for the implementer. My work focuses on designing new sketches and techniques that solve barriers to implementation, treating them as building blocks to address a wide range of problems rather than individual solutions for specific, stylized problems, and providing means for practitioners to easily optimize their choices of sketches and parameters. 

Hopefully, that gives an idea of what my research is about as well as some of the practical goals of the work. I’d like to think that my work is well-motivated by real problems I’ve seen, and I am always looking for more motivating problems from industry as well. So if you have any, drop me a line!

P.S. For those interested in some examples of my research: The NeurIPS paper Optimal Subsampling using Influence Functions shows how to construct optimal subsampling procedures for any parametric ML/stats model. My work on the CountMin sketch in KDD shows how to obtain optimal estimates, useful, tight error estimates instead of very loose bounds, and how to use these to choose the best sketch parameters. A collection of papers [1, 2, 3] on distinct counting and set operations address how to construct optimal counters and design sketches that can efficiently answer a multitude of distinct count queries, an important problem in some industrial applications, such as ad reporting / unique impression counting.
