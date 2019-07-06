---
layout: page
title: Training
---

* The samples of training set is first shuffled in random order, 
   and then split into batches per 128 samples
* Batch size refers to the number of training examples utilized 
    in one iteration. Essentially, the gradient and the neural 
    network parameters are updated after each batch.
* Batches are then feed into the model in random order to 
    avoid bias towards batches with larger index

{:refdef: style="text-align: center;"}
![image-title-here](/img/training.png){:class="img-responsive"}
{: refdef}