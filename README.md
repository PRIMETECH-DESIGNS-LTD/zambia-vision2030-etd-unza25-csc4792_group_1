<div align="center">
  <img src="https://th.bing.com/th/id/OIP.aZt5o1S31YdVKWcrxIBK0gHaKH?w=200&h=200&c=10&o=6&pid=genserp&rm=2" alt="Zambia Vision 2030 Logo" width="150">
  
  <h1>ZAMBIA VISION 2030 ETD CLASSIFIER</h1>
 <h3 style="color:blue;"><i>UNZA CSC 4792 (2024/25) - Group Project | Department of Computer Science and Informatics</i></h3>
</div>

## **1. Business Understanding**

### **1.1 Problem Statement**
Zambia’s Vision 2030 aims to transform the nation into a prosperous middle-income economy through sectoral
development. However, tracking progress is hindered by:
- **Fragmented data**: Emerging and Transformative Developments (*ETDs*) are siloed across
government portals, reports, and international databases.
- **Manual classification:** Current sector tagging of ETDs (e.g., agriculture, mining, ICT) is
inconsistent, delaying policy adjustments.
- **Limited visibility:** Policymakers lack a unified view of ETD distribution across Vision 2030’s 12
priority sectors.

### 1.2 Business Objectives
- Automate ETD classification with ≥90% accuracy
- Identify underfunded sectors through cluster analysis
- Develop public dashboard for transparency

### 1.3 Data Mining Goals

```python
from transformers import BertForSequenceClassification
model = BertForSequenceClassification(num_labels=12)
```
  
### 1.4 Success Criteria

- **Classification Accuracy**  
  - Achieve a macro average F1-score of ≥ 0.85 for the automated sector classification model.  
  - Validated through 10-fold cross-validation on held-out test data.  

- **Cluster Interpretability**  
  - Attain a Silhouette Score of ≥ 0.6 for unsupervised clustering of ETDs.  
  - Clusters must be at least 80% interpretable by domain experts in relation to Vision 2030 sectors.  

- **Policy Relevance**  
  - Ensure ≥ 90% of classified sectors align with Zambia’s Eighth *National Development Plan* (8NDP) priorities.  
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