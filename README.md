# Machine Learning Assignment-2

## Introduction
Nowadays we find the word “Transformers” everywhere in AI. As with all new technology, it is important to be able both to understand it and to be able to use it. In this assignment, you will be updating the demo notebooks (found in the files section of the course) with Transformer models.

In nutshell, attention is another mechanism that can be added to neural networks so that they can focus on the most important parts of the previous layer’s output. If you’d like to see more of the technical implementation, you can find a nice explanation here Links to an external site.. In 2017, Vaswani et al. Links to an external site. showed that you can create a neural network using only attention layers. They called this the transformer architecture. From there, a lot of new models such as BERT, GPT, and diffusion models were birthed. 

The more practical point of view is a bit more simple. A group called HuggingFace 🤗 (yes, including the emoji – actually the emoji is the name of the organization) was created to allow people to easily use these models. They have a lot of courses Links to an external site. and tutorials Links to an external site. that will allow you to use all of their packages in an easy manner, and we have seen HuggingFace material in class.

This might seem like too much for a single assignment, so we will try to point you to the relevant tutorials in the rest of the assignment.

## How this Assignment Works
You can choose one or both of the demo notebooks on which to work on. In order to get full credits for the assignment, you only have to do one of them. If you do both, you will get half the points of the one with the lowest points as bonus points.

You will create a new Jupyter notebook to write your code in.  You can also borrow code from the tutorialslinked in each section. Whatever you choose, don't forget to credit the original author and the dataset you're using!

Write any notes in a markdown file and upload your project to a GitHub repository. You should submit a link to the repo. If any of your models are too big for GitHub, you can upload them to a cloud service such as Google Drive, Dropbox, etc. and link to them either on your notebook or on the markdown file.

If you make any changes to the original code, state clearly in your markdown file the changes you made. 

There are 30 points on this assignment and 30 bonus points.  As usual, success is much less important than a good-faith attempt at completion and demonstrating understanding.  Focus first on getting the pipeline working end to end.

## Demo 2 – Chinese Word Segmentation
 

Part 1 – Transformers for Sequence Classification (7 points)
Here we want to compare how Transformers work when compared to other kinds of sequence to sequence networks, such as LSTMs. Follow the tutorial here Links to an external site. in order to implement a token classification model.

The tutorial uses DistilBERT, a smaller version of BERT designed to be used when we have less memory available. BERT itself is one of the most popular Transformer models both for sequence and for token classification.

 

Part 2 – Using BERT with Our Data (16 points)
The huggingface tutorial uses both an English dataset and a model pretrained in English. Change the code so that it can use the CONLL-U dataset from the demo notebook.

One of the major issues that you might find is that just changing the dataset will not yield the results we would expect. Because of that, you might also have to change the model you’re using. I wasn’t able to find a reasonably documented version of DistilBERT for Chinese, but HuggingFace has a Chinese BERT Links to an external site. available.

Another thing to keep in mind is that BERT already segments the words as it things they should be segmented, so you will probably have to find a workaround in order to avoid the task being trivial (and to get a single label from each of your characters).

 

Part 3 – Performance Analysis (7 points)
Do a comparison between both models and how differently they perform. We are assuming that most of you don’t read Chinese, so we are not expecting much in the area of qualitative analysis.

 
