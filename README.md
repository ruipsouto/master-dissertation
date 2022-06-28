# Query Optimizers Based on Machine Learning Techniques

Query optimizers are considered one of the most relevant and sophisticated components in a database management system. However, despite currently producing nearly optimal results, optimizers rely on statistical estimates and heuristics to reduce the search space of alternative execution plans for a single query. As a result, for more complex queries, errors may grow exponentially, often translating into sub-optimal plans resulting in less than ideal performance. Recent advances in machine learning techniques have opened new opportunities for many of the existing problems related to system optimization. 

This document proposes a solution built on top of PostgreSQL that learns to select the most efficient set of optimizer strategy settings for a particular query. Instead of depending entirely on the optimizer's estimates to compare different plans under different configurations, it relies on a greedy selection algorithm that supports several types of predictive modeling techniques, from more traditional modeling techniques to a deep learning approach.

The system is evaluated experimentally with the standard TPC-H and Join Ordering Benchmark workloads to measure the cost and benefits of adding machine learning capabilities to traditional query optimizers.

**Keywords** Database tuning, machine learning, query optimization
