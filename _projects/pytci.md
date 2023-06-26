---
layout: project
title: PyTCI
photo: /assets/pytci.png
tag: pytci
type: research
code: https://github.com/naplab/PyTCI
sort_key: 2
subtitle: Toolbox for analyzing temporal integration window of time-series models.
description: "A python toolbox to analyze the temporal integration windows of
    computational models (e.g., artificial neural networks) that process 
    time-series input."
---

A python toolbox to analyze the temporal integration windows of neural 
networks that process time-series input. Integration windows are defined as 
the time window within which stimuli alter a sensory response and outside of 
which stimuli have little effect. Integration windows provide a simple and 
general way to define the analysis timescale of a response. We estimate 
integration windows by presenting segments of natural stimuli in two different 
pseudorandom orders, such that the same segment occurs in two different 
contexts (is surrounded by different segments). We then estimate the smallest 
segment duration outside of which stimuli have little effect on the response.

The TCI paradigm was initially developed to estimate integration windows for 
biological neural systems ([Norman-Haignere et al, 2022](
https://www.nature.com/articles/s41562-021-01261-y)). The method however 
can be applied to any sensory response, and we have recently used the method 
to understand how deep speech recognition systems learn to flexibly integrate 
across multiple timescales (Keshishian et al, 2021).
