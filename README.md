# Embeddings Aggregation Techniques Based on Representational Similarity Measures

This repository contains the code for a research paper "Embeddings Aggregation Techniques Based on Representational Similarity Measures", which was my Bachelor's thesis.

### About the code

To reproduce the code, no preliminary preparation of the environment or data is required; all the necessary dependencies can be found in the notebooks. The entire pipeline is divided into four logical parts:

1. Calculation of quality and representational similarity measures on the training set. This notebook contains a quality calculation on the selected MTEB benchmark task for each of the 12 layers of the selected BERT-like model, as well as a calculation of embedding similarity metrics between each pair of layers. As a result of its execution, two files with corresponding tables become available, which are later used to obtain weights. 
2. Calculating weights based on similarity measures. In this part, according to the described method, optimal weights are selected for individual embedding similarity metrics, as well as their combinations. The resulting weights are saved to a file. 
3. (Optional) Obtaining optimal weights using optuna. If you have sufficient computing resources, you can try to find the optimal weights using optuna. 
4. Testing of the acquired weights. In this laptop, the quality of the combination, compiled using the weights from points 2-3, is measured on a test set.


#### Fulfilled by:
Avgustyonok Alina Alekseevna \
Student of the Group БПМИ211 \
Faculty of Computer Science, HSE University

#### Project Supervisor:
Savchenko Andrey Vladimirovich \
Doctor of Technology, Senior Researcher \
Faculty of Computer Science, HSE University
