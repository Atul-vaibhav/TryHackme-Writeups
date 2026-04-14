# 🧠 TryHackMe Write-up: Ai Models & Data

## 📅 Date
14 April 2026

## 🔗 Room Link
[https://tryhackme.com/room/aimodelsdata](https://tryhackme.com/room/aimodelsdata)

---

## 🎯 Learning Objective
- Understand where AI training data comes from and the security risks introduced by poor data provenance
- Recognise how PII and sensitive credentials can become permanently embedded in model weights through large-scale web scraping
- Understand how key model-building decisions (overfitting, quantisation, and federated learning) each introduce distinct security risks
- Understand the inheritance problem and what organisations unknowingly take on when fine-tuning pre-trained models
- Recognise why trained models are opaque black boxes, and what model cards do (and fail to do) to address this
---

## Task 2 

- Source of AI Training Data -
  1. Web Scraping - Automated crawls of public internet content.  Trust - Low
  2. Licensed Datasets - Data Purchased or agreed with social media platforms.  Trust - Medium
  3. Synthetic Data - Ai-generated content used to train further AI Systems.  Trust - Varible
  4. Internal corpora - Company knowledge bases, support transciptions , clinical notes used for fine-tuning.   Trust - Higher

- Data Provenance - Ability to answer three questions -
-     1. Where did it came from ?
-     2. When was it collected?
-     3. Has it been modified Since ?

Room Answers - Data Provenance, Common Crawl, ML-BOM

## Building The models - 

- Epochs - One complete pass of the training lagorithm through the entire dataset.
- Overfitting - A situation when model stops learning general patterns and starts memorising trainign data speciafically. A overfit model performs well on training data but poor on other data.
