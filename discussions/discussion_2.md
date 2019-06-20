---
title: "Discussion 2"
author: "Olga Shiligin"
date: "20/06/2019"
output: html_document
---


Task 2: For this discussion item, please watch the following talk and summarize what you found to be the most important or interesting points.
------

Video Takeaways:
----------------

The effectiveness of industrial scale recommender system requires not only advanced mathematical techniques, but also significant data management skills.

Mathematical Techniques:
------------------------

There are various recommendations techniques:

   - Manual curation for small catalogs
   - Manually Tag Attributes (using expert knowledge), not very scalable though.
   - Audio content, text Analysis
   - Collaborative filtering

Spotify uses mostly collaborative filtering and implicit matrix factorization for dimensionality reduction. The idea of matrix factorization is basically to take a large (or potentially huge) matrix and factor it into some smaller representation of the original matrix. We end up with two or more lower dimensional matrices whose product equals the original one. Implicit factorization unlike explicit factorization uses implicit data which is gathered from the users behaviour, with no ratings or specific actions needed. Using implicit data we focus on what we know the user has consumed and the confidence we have in whether or not they like any given item. For example the original Netflix challenge focused only on explicit data but they’re now relying more and more on implicit signals. For explicit data we can apply SVD or PLSA and treat missing values as just unknown fields that we should assign some predicted rating to, but we can not do same things with implicit data. The solution for that problem is to use Alternative Least Square regression (ALS). ALS is an iterative optimization process where we for every iteration try to arrive closer and closer to a factored representation of our original data.


Data Management Challenges:
--------------------------

Hadoop definition from their home page:"The Apache Hadoop software library is a framework that allows for the distributed processing of large data sets across clusters of computers using simple programming models". The major problem of Hadoop is its Input / Output (I/O) performance. Spark is a fast and general compute engine for Hadoop data which addresses Hadoop's performance issue by caching the data in memory. Spark provides feature reach API for map/reduce operations, ML, ETL processes and performance tuning. 
However, performance comes for a price. Spark performance tuning in most cases is about reducing memory consumption and data shuffling across Spark nodes, which can often be cumbersome as it requires knowledge of sophisticated algorithms that Spark is using for running computational processes split in multiple tasks running in parallel.  
