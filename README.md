<div align="center">
  <img src="https://th.bing.com/th/id/OIP.aZt5o1S31YdVKWcrxIBK0gHaKH?w=200&h=200&c=10&o=6&pid=genserp&rm=2" alt="Zambia Vision 2030 Logo" width="150">
  
  <h1>Zambia Vision 2030 ETD Classifier</h1>
 <h3 style="color:blue;"><i>UNZA CSC 4792 (2024/25) - Group Project | Department of Computer Science</i></h3>
</div>

## 1. Business Understanding

### 1.1 Problem Statement
- Fragmented ETD data across government portals
- Inconsistent manual classification processes
- Limited visibility into sectoral distribution

### 1.2 Business Objectives
- Automate ETD classification with ≥90% accuracy
- Identify underfunded sectors through cluster analysis
- Develop public dashboard for transparency

  ### 1.3 Data Mining Goals

```python
from transformers import BertForSequenceClassification
model = BertForSequenceClassification(num_labels=12)
```
Vision 2030 sectors
  
### 1.4 Success Criteria

- **Classification Accuracy**  
  - Achieve a macro average F1-score of ≥ 0.85 for the automated sector classification model.  
  - Validated through 10-fold cross-validation on held-out test data.  

- **Cluster Interpretability**  
  - Attain a Silhouette Score of ≥ 0.6 for unsupervised clustering of ETDs.  
  - Clusters must be at least 80% interpretable by domain experts in relation to Vision 2030 sectors.  

- **Policy Relevance**  
  - Ensure ≥ 90% of classified sectors align with Zambia’s Eighth National Development Plan (8NDP) priorities.  
  - Verified through manual review by Ministry of Finance experts.  

- **Operational Efficiency**  
  - Reduce manual tagging time by at least 70% compared to current processes.  
  - Measured using a time-motion study.  

- **Dashboard Performance**  
  - Ensure public-facing dashboard loads in ≤ 2 seconds under standard network conditions.  
  - Measured through automated performance testing.  

  ### 1.5 Data Sources
- Zambia Development Agency API
- World Bank Projects Database
- 8th National Development Plan PDF