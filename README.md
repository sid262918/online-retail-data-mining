# Online Retail Data Mining

## Overview
This project uses an Online Retail dataset to examine the purchasing patterns of customers. The objective is to find out which items are typically bought by customers at the same time and assess how close the relationships among them are through mining techniques like frequent itemset mining and association rule mining.

Start here: **main_notebook.ipynb**

## Research Questions
- What itemset appear in the Online Retail dataset when varying the support threshold?
- How do the confidence and lift compare when dealing with association rules evaluated from the retail transactions?
- Can Sequential patterns show purchasing relationships that would not be captured by unordered frequent itemsets?


## Project Video
https://youtu.be/gKksu2jxWkE


## Data
- **Dataset:** Online Retail Dataset  
- **Source:** Kaggle  
- **Description:** Transaction-level data from a UK-based online retail store  

### Preprocessing Steps:
- Removed cancelled transactions  
- Removed negative quantities and prices (returns)  
- Grouped data into transaction baskets using `InvoiceNo`  


## How to Reproduce
- Built using **Google Colab**
- Install dependencies:
  - Pandas
  - numpy
  - mlxtend


pip install -r requirements

### Run Order:
1. Open and run `main_notebook.ipynb`


## Key Dependencies
- Python 3.x  
- pandas  
- numpy  
- mlxtend  

(Full list available in `requirements.txt`)


## Repo Structure
├── main_notebook.ipynb
├── checkpoint_1.ipynb
├── checkpoint_2.ipynb
├── requirements.txt
└── README.md


## Results Summary
The analysis shows that customer purchasing behavior has a long-tail distribution, where a small number of products dominate the transactions while most of the products appear less often. Strong association rules were found between similar products, like different types of teacup sets being frequently purchased together. While these methods successfully identify strong patterns, the results are heavily influenced by popular items, which can limit the discovery of less frequent but meaningful relationships.
