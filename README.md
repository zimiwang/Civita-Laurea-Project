# The Effects of Supervised Modeling and Unsupervised Hierarchical Clustering for Topic Clustering as They Apply to Educational Videos on Mathematics
![image](https://github.com/zimiwang/Civita-Laurea-Project/assets/56045330/d361e0c8-51bf-4102-8e02-3258f96947b9)


## Introduction

This project, spearheaded by Ziming Wang from Idaho State University, delves into the clustering of scripts from educational mathematical videos to discern the predominant topic of each video. Utilizing advanced Natural Language Processing (NLP) techniques, this undergraduate endeavor aims to categorize video scripts without pre-existing labels by applying various models and methodologies to extract meaningful data and insights.

## Objective

The primary goal is to leverage unsupervised learning to assign topics to video scripts, facilitating an organized and insightful grouping of educational content. This approach allows for a deeper understanding and easier navigation of educational materials in mathematics.

## Workflow and Methodology

### Preliminary Research

Initial steps included a comprehensive exploration of Natural Language Processing (NLP), focusing on its ability to enable computers to understand text and spoken words as humans do.

### Topic Modeling

- **Latent Dirichlet Allocation (LDA) Model**: As a starting point, the LDA model was applied to analyze documents (video scripts) and assign topics based on statistical information. Despite its usefulness, the LDA model's results became overly generalized with an increase in script volume, leading to a search for more context-sensitive solutions.

- **BERT Model**: Although the Bidirectional Encoder Representations from Transformers (BERT) model showed promise due to its deep understanding of context, it proved less effective for long text classification tasks found in our scripts.

- **KeyBERT Model**: This model was introduced to overcome the limitations of BERT by focusing on keyword extraction. By integrating KeyBERT with a mathematics keyword corpus, we were able to enhance script classification significantly.

### Classification and Clustering

- **XGBoost Model**: This phase involved categorizing scripts based on teaching style ("theoretical" or "applied") and subject matter (calculus or precalculus). The XGBoost model, coupled with manual data labeling and SMOTE for data imbalance handling, achieved an impressive ~95.5% accuracy in predicting teaching styles and subjects.

- **BERTopic Model**: Employing BERTopic, the project further refined topic extraction and clustering, utilizing algorithms like UMAP, HDBSCAN, and hierarchical clustering to group scripts by similarity and thematic content.

## Results

Through a meticulous process of cleaning scripts, manual classification, and sophisticated model application, the project successfully grouped educational scripts into coherent categories, each tagged with relevant keywords. This unsupervised approach culminated in a rich set of classified and clustered scripts, making educational content more accessible and navigable.

## Conclusion

This project represents a significant step forward in the application of NLP and machine learning to educational content, demonstrating the power of unsupervised learning in uncovering insights from unstructured data. By classifying and clustering mathematical video scripts, we've created a valuable resource for educators and learners alike, enabling more targeted and efficient educational experiences.

### Project Team

**Ziming Wang**
- Role: Coordination of research efforts and primary development of the LDA and KeyBERT models.
- Affiliation: Undergraduate Student, Idaho State University

**David Lindeman**
- Role: Coordination of research efforts and primary development of the LDA and KeyBERT models.
- Affiliation: Undergraduate Student, Idaho State University

### Faculty Advisor

**Dr. Xiaoxia Xie**
- Affiliation: Professor, Mathematics Department, Idaho State University

### Project Provider

**Laura Sánchez Fernández**
- Affiliation: Civita Laurea, Canada
