# ComRH--Combining Representation Learning and Classic Heuristics for Link Prediction.
===============================================================================
About
-----
This repository supports the following work:
Combining Representation Learning and Classic Heuristics for Link Prediction.

In this work, we aim to study the Combination of the best of both Representation learning and link Heuristics to boost the performance of link prediction.
ComRH separately encodes link heuristics into trainable embedding vectors and directly combine them with the outputs of representation learning. Also, we propose an effective and scalable Sparse Mask Graph Transformer (SMGT). Theoretically, graph Transformers including SMGT still belong to the family of neighborhood aggregation-based GNNs but their neighborhood contains not only locally linked nodes but also global nodes, which leads to a more expressive power of graph Transformer than classic GNNs. In particular, SMGT uses a mask to restrict the size of neighborhood of each node, which allows the attention to be computed in sparse setting, making SMGT scalable for large graph.

We conduct experiments on four link prediction datasets from  Open Graph Benchmark (OGB). ComRH outperforms all baselines including subgraph-based methods and significantly exceeds the top 1 results in the OGB leaderboard by $3.52\%$ Hits@20 on ogbl-ddi, $3.42\%$ Hits@50 on ogbl-collab, $9.32\%$ Hits@100 on ogbl-ppa, and $0.11\%$ MRR on ogbl-citation2. This demonstrates that link heuristics provide ComRH with different yet effective information to boost the link prediction performance, and the combination method in ComRH is more effective than prior methods including subgraph-based methods. Further experiments show that ComRH with SMGT achieves superior performances over its competitors. Also, we observe that link heuristics could contribute much more to the prediction in sparse graphs than very dense graphs.
