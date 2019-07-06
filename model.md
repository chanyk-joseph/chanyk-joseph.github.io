---
layout: page
title: Neural Network Model
---

We make use of two layers of bidirectional LSTM as the input sequence encoder, and pass the encoded result to the 
self-attention layer extracted from BERT. Finally, the output from attention layer would be condensed into our prediction target, i.e. log return of the next timestep.

Bi-LSTM is an enhancement to the LSTM model which is a commonly used machine learning model for time series prediction.
The series of data is encoded from **Left-to-Right** and also **Right-to-Left** in order to preserve more sequential relationships.
{:refdef: style="text-align: center;"}
![image-title-here](/img/bi-lstm.jpg){:class="img-responsive"}
{: refdef}

Bidirectional Encoder Representations from Transformers (BERT), published by google in Oct, 2018, is a model designed to pre-train deep bidirectional representations from unlabelled text by jointly conditioning on both left and right context in all layers. BERT makes use of **self-attention** which has been adopted successfully in a variety of tasks such as reading comprehension, abstractive summarization, textual entailment and learning task-independent sentence representations. Self-attention is an intra-attention mechanism for relating different positions of a single sequence in order to compute a representation of the sequence.
{:refdef: style="text-align: center;"}
![image-title-here](/img/self-attention.png){:class="img-responsive"}
{: refdef}