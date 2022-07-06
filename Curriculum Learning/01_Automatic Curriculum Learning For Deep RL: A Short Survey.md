# [Automatic Curriculum Learning For Deep RL: A Short Survey](https://arxiv.org/pdf/2003.04664.pdf)

This is a short survey on Curriculum Learning, the ambition of this work is dual: 1) to present
a compact and accessible introduction to the Automatic Curriculum Learning literature and 2) to
draw a bigger picture of the current state of the art in ACL to encourage the cross-breeding of existing
concepts and the emergence of new ideas.

## Motivation
Sometimes the target tasks cannot be solved directly (e.g. too hard or sparse rewards). In that case,
ACL can be used to pose auxiliary tasks to the agent, gradually guiding its learning trajectory from simple to difficult
tasks until the target tasks are solved.

## What does CL control
### CL for Data collection
During data collection, CL organizes the sequential presentation of tasks as a function of the agent’s capabilities. 
### CL for Data exploitation
