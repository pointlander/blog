---
title: "Scalable Models"
date: 2018-11-15T21:43:27-07:00
draft: false
---

The author of [Gorgonia](https://github.com/gorgonia/gorgonia), a neural network library, had an interesting [Strange Loop talk](https://www.thestrangeloop.com/2018/a-funny-thing-happened-on-the-way-to-reimplementing-alphago.html) about reimplementing [AlphaGo](https://en.wikipedia.org/wiki/AlphaGo). The problem they ran into is that it would have cost them $70,000 to train a competitive model, so they focused on training their algorithm for games with a smaller board. What if a small neural network could be scaled to work on a larger board? The approach that I propose is based on [program synthesis](https://en.wikipedia.org/wiki/Program_synthesis). Converting a neural network into a program has been demonstrated in this [paper](https://arxiv.org/abs/1804.02477). A neural network trained on a smaller Go board could be converted into a program, and the program could then be modified to work on a larger Go board. A summary of program synthesis work can be found [here](https://alexpolozov.com/blog/program-synthesis-2018/).
