---
layout: project
title: dSTRF
photo: /assets/dstrf.png
tag: dstrf
type: research
code: https://github.com/naplab/DSTRF
webpage: http://naplab.ee.columbia.edu/dstrf.html
sort_key: 1
subtitle: Toolbox for analyzing local spectro-temoral receptive field of neurons.
description: "A python toolbox to analyze feed forward neural networks trained
    to predict biological neural responses to sound, by computing the locally
    linear operations they perform on the input."
---

A python toolbox for dynamic spectrotemporal receptive field (dSTRF) analysis, as 
introduced in Keshishian et al (2020). In short, dSTRF is a method 
to analyze which parts of the input at any time point are being used by a 
feed-forward deep neural network to predict the response.

In mathematical terms, for a nonlinear model $$f(\cdot)$$, input at time 
$$t$$, $$X_t$$, and output at time $$t$$, $$Y_t = f(X_t)$$, the dSTRF is the 
locally linear transformation $$W_t$$, such that: $$Y_t = W_t X_t$$. Now, if 
$$f(\cdot)$$ is a linear function, $$W_t$$ will be the same for all $$t$$. If 
not, the linearized function applied to the input ($$W_t$$) will depend on the 
given stimulus ($$X_t$$), which is the case in a deep neural network.

A linear function mapping the auditory stimuli in the spectrotemporal domain 
(i.e., auditory spectrograms) to the neural activity recorded from the 
biological brain is called a spectrotemporal receptive field (STRF). Since 
we use a nonlinear mapping between the stimulus and response, and characterize 
it as a locally linear function at each time point, we call this a dynamic 
spectrotemporal receptive field (dSTRF).
