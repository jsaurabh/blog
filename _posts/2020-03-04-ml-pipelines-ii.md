---
title: "Machine Learning Pipelines - Part II"
summary: "Dataset exploration. Extracting meaningful patters and trends from data"
layout: post
toc: true
comments: true
categories: [ml, mlpa]
hide: false
---
# Machine Learning Pipelines - Part II

In [Part I](https://jsaurabh.dev/ml/mlpa/2020/02/26/ml-pipelines.html), we went ahead and wrote a rudimentary version of the pipeline we'll be using for the webapp. 

{% include alert.html text="It's not a pipeline" %}

In this post, we'll focus on acquiring an initial dataset and extract and generate features.

## Writing Better Questions

Following along with the book, we want to build an editor that lets its users write better questions. Before we go and build a model, the first step is playing around with the data. That begs the question, what kind of dataset should we be looking at?

Some good places to find datasets are [Kaggle](https://www.kaggle.com/datasets), the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php) as well as the [AWS Open Data registry](https://registry.opendata.aws/). 

For our use case, we'll go ahead with StackExchange [dump](https://archive.org/download/stackexchange) specifically the Writers dump [here](https://ia800107.us.archive.org/view_archive.php?archive=/27/items/stackexchange/writers.stackexchange.com.7z)

Each of these dumps is an XML file with the headers and attributes containing the actual info we need. We need to extract raw text, and this is where we'll write a basic pipeline to get the data we need.
