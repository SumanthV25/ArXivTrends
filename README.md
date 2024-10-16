
# Big Data Analytics: Research Trends & Recommendation System



## Table of Contents
1. [Overview](#overview)
2. [Motivation](#motivation)
3. [Dataset](#dataset)
4. [Methodology](#methodology)
5. [Results](#results)
6. [Future Work](#future-work)
7. [Installation](#installation)
8. [Usage](#usage)
9. [Contributors](#contributors)

---

## Overview

This project explores **research trends and recommendation systems** using a massive dataset from Arxiv. We focused on analyzing research paper metadata, extracting insights into publication trends, and building a **research paper recommendation engine** based on user inputs (paper titles). The system leverages **Content-Based Filtering** combined with **NLP techniques** to suggest relevant research papers from the Arxiv dataset.

---

## Motivation

In the modern age of **information overload**, finding relevant research papers can be overwhelming. This project was developed to assist researchers in navigating through vast datasets, identifying key research trends, and discovering relevant papers efficiently. It was built with the goal to uncover **hidden patterns, collaborations, and trends** within the research community.

---

## Dataset

The dataset used for this project was sourced from **Arxiv**, comprising over **2.3 million research papers**. This dataset includes fields like title, abstract, authors, publication date, and category. We used a subset of this data focused on the **Computer Science** domain, which contains over 621,547 entries.

The datasource of ArXiv papers is from Kaggle: https://www.kaggle.com/datasets/Cornell-University/arxiv

---

## Methodology

Our approach involved several key steps:

1. **Data Collection and Preprocessing**: 
   - Converted the Arxiv JSON dataset into a manageable dataframe using **Dask** and other libraries.
   - Cleaned the data by handling missing values and performing feature engineering on key columns like `authors` and `abstract`.

2. **Exploratory Data Analysis (EDA)**: 
   - Visualized key trends in research publications over the years.
   - Conducted **authorship analysis**, exploring the most prolific authors and collaborative trends.
   - Investigated **topic analysis** to understand the distribution of research fields.

3. **Recommendation Model**:
   - Built using a **Multi-Layer Perceptron (MLP)** model with **sentence transformers** to embed and match paper titles.
   - **Cosine similarity** is used to recommend papers based on the user's input.



---

## Results

- The **recommendation system** provides users with the top 5 most similar papers based on the cosine similarity of embeddings.
- Key insights into **publication trends** were uncovered, especially in the **Computer Science** field, showing a steady rise in research outputs over the years.

- 
  ![image](https://github.com/user-attachments/assets/158c4ac1-a058-42f2-a6ef-9ecdcd74f5a9)


---

## Future Work

The system can be expanded further by:
- Incorporating **citations and author collaboration networks** for more accurate recommendations.
- Applying the model to other research fields beyond Computer Science.
- Improving the model's ability to handle a larger dataset for real-time recommendations.

---

## Installation

### Requirements
- **Python 3.8+**
- **TensorFlow**
- **Scikit-learn**
- **Numpy**
- **Pandas**
- **Dask**
- **Sentence Transformers**
- **Matplotlib** (for plotting)

Install the required packages using pip:

```bash
pip install -r requirements.txt
```


## Contributors

- **V. Sumanth**  
  Student, **BML Munjal University**  
  Supervisor: **Dr. Yogesh Gupta**

Feel free to contribute by submitting issues or pull requests.

