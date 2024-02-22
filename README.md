
# About this dataset

This dataset was created with two purposes :
1. Unveil identity biases in a toxicity detection model for written videogame chat
2. Reflect the type of lines found in a written game chat

The dataset contains a total of 16,008 lines, created from 22 sentence templates and a set of 46 identity-related terms.
A full description of the dataset creation method is available in the [EMNLP 2023 article](https://aclanthology.org/2023.emnlp-industry.26/).

# Structure of the dataset

The dataset contains 10 columns :

- **chat_line** : synthetic chat line made from a sentence template and a term or combination of terms that may convey identity biases
- **template** : the sentence template used to create this chatline
- **word1**, **word2** : the words used to fill the tag in the sentence template
- **lem1**, **lem2** : the lemmatized version of word1, word2
- **cat1**, **cat2** : the categories associated to word1, word2
- **manual_annotations** : toxicity annotations that were obtained from human annotators. Only 1,363 lines have a value in this column.
- **annotations** : the ground truth labels. These labels were obtained from a propagation using a random forest algorithm, trained on the 1,363 manually annotated lines.

For both the columns **manual_annotations** and **annotations** :

- 0 = non-toxic line
- 1 = toxic line

# Cite this dataset

If you use this dataset, please cite the following paper : 

Van Dorpe, J., Yang, Z., Grenon-Godbout, N., & Winterstein, G. (2023). Unveiling Identity Biases in Toxicity Detection: A Game-Focused Dataset and Reactivity Analysis Approach. In M. Wang & I. Zitouni (Eds.), Proceedings of the 2023 Conference on Empirical Methods in Natural Language Processing: Industry Track (pp. 263–274). Association for Computational Linguistics. https://doi.org/10.18653/v1/2023.emnlp-industry.26


© [2023] Ubisoft Entertainment. All Rights Reserved.