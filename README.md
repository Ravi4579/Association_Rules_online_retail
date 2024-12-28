# Association Rules Mining - Market Basket Analysis

This repository contains the implementation of association rule mining using the Online Retail dataset. The project applies the Apriori algorithm to uncover interesting relationships between products purchased together, with a focus on analyzing customer purchasing behavior.

## Objective
The objective of this project is to introduce rule mining techniques, specifically focusing on market basket analysis, and provide hands-on experience using the Apriori algorithm for association rule mining.

---

## Dataset
**Online Retail Dataset**:
The dataset used in this project consists of transactional data that records purchases from an online retail store.

### Dataset Preprocessing
1. **Handling Missing Values**: Removed rows with missing or null values.
2. **Duplicate Removal**: Removed duplicate entries from the dataset.
3. **Data Formatting**: Transformed data into a suitable format for association rule mining, such as a transactional format or binary matrix.

---

## Methodology

### Tools and Libraries
- **Python**
- **Pandas**: For data manipulation and preprocessing.
- **Mlxtend**: For implementing the Apriori algorithm and generating association rules.

### Implementation Steps
1. **Data Preprocessing**:
    - Handled missing values and duplicates.
    - Formatted the dataset to suit association rule mining requirements.

2. **Association Rule Mining**:
    - Applied the Apriori algorithm to identify frequent itemsets.
    - Set thresholds for support, confidence, and lift to filter meaningful rules.

3. **Analysis**:
    - Analyzed the rules to identify interesting patterns and relationships.
    - Interpreted results to provide insights into customer purchasing behavior.

---

## Analysis and Insights
### Key Metrics
- **Support**: Measures how frequently an itemset appears in the dataset.
- **Confidence**: Measures the likelihood of an item being purchased given another item is purchased.
- **Lift**: Indicates the strength of a rule over random co-occurrence.

### Observations
- Identified frequently purchased product combinations.
- Derived actionable insights into customer preferences and cross-selling opportunities.

---

## Interview Questions and Answers

### 1. What is lift and why is it important in Association Rules?
**Answer**: Lift is a measure of how much more likely two items are purchased together compared to if they were independent. A lift value greater than 1 indicates a strong positive association, whereas a value less than 1 suggests a negative or no association. Lift is crucial as it highlights the strength and relevance of a rule.

### 2. What is support and confidence? How do you calculate them?
- **Support**: Proportion of transactions containing a particular itemset.
  - Formula: `Support = (Number of transactions containing the itemset) / (Total number of transactions)`

- **Confidence**: Probability of a consequent item being purchased when the antecedent item is purchased.
  - Formula: `Confidence = (Support of antecedent and consequent) / (Support of antecedent)`

### 3. What are some limitations or challenges of Association Rules Mining?
- High computational cost for large datasets.
- Difficulty in setting optimal thresholds for support, confidence, and lift.
- Rules may lack business relevance without proper domain knowledge.
- Sparsity of transactional data can affect rule quality.

---

## How to Run the Code
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/association-rules-mining.git
   ```
2. Install the required dependencies:
   ```bash
   pip install pandas mlxtend
   ```
3. Run the Python script to preprocess the data and generate association rules.

---

## Folder Structure
```
|-- data/                  # Contains the dataset
|-- notebooks/             # Jupyter notebooks for implementation
|-- src/                   # Python scripts for data preprocessing and analysis
|-- results/               # Output of rules and analysis
|-- README.md              # Project documentation (this file)
```
