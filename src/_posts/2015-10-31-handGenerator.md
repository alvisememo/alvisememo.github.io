---
layout: post
title:  "Hand generator"
date:   2015-10-31 00:00:00 -0800
---

Hello, In this post I will give a brief presentation of the software
*HandGenerator*, that I created to generate the synthetic dataset
used in the publication (A.Memo, L. Minto and P. Zanuttigh, [“Exploiting 
Silhouette Descriptors and Synthetic Data for Hand Gesture Recognition”,
STAG: Smart Tools & Apps for Graphics
](http://lttm.dei.unipd.it/downloads/handposegenerator/images/paper.pdf).

To download and test the library, to see it's capabilities, please follow
this link to the LTTM Laboratory at the University of Padua,
[HandGenerator@LTTM](http://lttm.dei.unipd.it/downloads/handposegenerator).

The library enables the user to have an intuitive GUI to set up the hand
pose, and then recursively generate a large dataset with its parameters.
The possibility for customization allow for a wide field of usage, from
color-based datasets to depth-based (as the one used in the paper above):
this is done exploiting the possibility of using custom shaders for the
OpenGL pipeline that render the 3D model, and in this case the results
are shown below.

![](/assets/handgenerator-both.png){:height="200px"}
![](/assets/handgenerator-g1s.png){:height="200px"}
![](/assets/handgenerator-g6s.png){:height="200px"}
![](/assets/handgenerator-g13s.png){:height="200px"}