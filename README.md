# Drug-Drug-Interactions-Prediction
Jupyter Notebooks with Experiments for DDIs Prediction and Plot creation to compare different models (Network vs Chemical approach)

# Prerequisites

1. DrugBank Dataset (full dataset xml file and structures.sdf).
2. Mol2Vec pre-trained model (model_300dim.pkl): https://github.com/samoturk/mol2vec/tree/master/examples/models
3. conda_list.txt contains the full list of packages that were used in the conda environment for the experiments. Newest versions of these packages may be incompatible with the notebook code.

# Instructions

The drugbank_experiments.ipynb file contains python code blocks for:
1. DrugBank Dataset Extraction: The original dataset is extracted, augmented, filtered and, finally, stored in dataframe objects.
2. Mol2Vec Experiment: mol2vec embeddings are produced in order to create positive and negative samples. The sample set is split into train. validation and test sets, and a simple Feed Forward neural network is used for training and testing.
3. Node2Vec Experiment. NetworkX is used to create a graph, and similarly to Mol2Vec experiment we produce positive and negative sampeles and then proceed to train and test a NN.
4. Hybrid Experiment.

At the end of each experiment section, we provide code for plot creation.
