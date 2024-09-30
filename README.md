# Integrating Social Determinants of Health into Knowledge Graphs: Evaluating Prediction Bias and Fairness in Healthcare

### 🦸‍ Abstract
Social determinants of health (SDoH) play a crucial role in patient health outcomes, yet their integration into biomedical knowledge graphs remains underexplored. This study addresses this gap by constructing an SDoH-enriched knowledge graph using the MIMIC-III dataset and PrimeKG. We introduce a novel fairness formulation for graph embeddings, focusing on invariance with respect to sensitive SDoH information. Via employing a heterogeneous-GCN model for drug-disease link prediction, we detect biases related to various SDoH factors. To mitigate these biases, we propose a post-processing method that strategically reweights edges connected to SDoHs, balancing their influence on graph representations. This approach represents one of the first comprehensive investigations into fairness issues within biomedical knowledge graphs incorporating SDoH. Our work not only highlights the importance of considering SDoH in medical informatics but also provides a concrete method for reducing SDoH-related biases in link prediction tasks, paving the way for more equitable healthcare recommendations.

### 📝 Requirements
The experiment is implemented on Google Colab, utilizing a T4 GPU.

To run the experiment, ensure you have the Deep Graph Library ([DGL](https://www.dgl.ai/)) installed. You can do so by running the following command:

```bash
pip install dgl -f https://data.dgl.ai/wheels/torch-2.3/cu121/repo.html
