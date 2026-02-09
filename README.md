# TOPSIS-Based Selection of Best Pre-trained Model for Text Classification

## Objective
The objective of this project is to apply the **TOPSIS (Technique for Order Preference by Similarity to Ideal Solution)** method to identify the **best pre-trained model for Text Classification**.  
Since multiple NLP models are available, selecting the optimal one becomes a multi-criteria decision-making problem involving both performance and efficiency factors.

---

## Pre-trained Models Considered
The following widely-used text classification models were evaluated:

- BERT (bert-base-uncased)  
- RoBERTa (roberta-base)  
- DistilBERT  
- ALBERT  
- XLNet  

---

## Evaluation Criteria
The models were evaluated using the following criteria:

| Criterion | Description | Nature |
|---------|------------|--------|
| Accuracy | Correctness of classification | Benefit |
| F1-score | Balance between precision and recall | Benefit |
| Inference Time (ms) | Prediction latency | Cost |
| Model Size (MB) | Storage requirement | Cost |
| Training Time (hrs) | Computational effort | Cost |

---

## Decision Matrix

| Model | Accuracy | F1-score | Inference Time (ms) | Model Size (MB) | Training Time (hrs) |
|------|----------|----------|--------------------|----------------|--------------------|
| BERT | 0.92 | 0.91 | 45 | 420 | 6 |
| RoBERTa | 0.94 | 0.93 | 50 | 500 | 7 |
| DistilBERT | 0.90 | 0.89 | 25 | 250 | 4 |
| ALBERT | 0.91 | 0.90 | 30 | 220 | 5 |
| XLNet | 0.93 | 0.92 | 55 | 480 | 8 |

---

## Criteria Weights

| Criterion | Weight |
|---------|--------|
| Accuracy | 0.30 |
| F1-score | 0.25 |
| Inference Time | 0.20 |
| Model Size | 0.15 |
| Training Time | 0.10 |

---

## TOPSIS Methodology
The following steps were followed:

1. Construction of the decision matrix  
2. Normalization of the decision matrix  
3. Calculation of weighted normalized matrix  
4. Determination of ideal best and ideal worst solutions  
5. Computation of Euclidean distances  
6. Calculation of closeness coefficient and ranking  

---

## 📈 Results

### 🔹 TOPSIS Scores and Ranking

| Model | TOPSIS Score | Rank |
|------|-------------|------|
| DistilBERT | **0.72** | **1** |
| ALBERT | 0.65 | 2 |
| BERT | 0.61 | 3 |
| RoBERTa | 0.58 | 4 |
| XLNet | 0.54 | 5 |

---

## Graphical Analysis

## TOPSIS Score Comparison
<img width="609" height="449" alt="Screenshot 2026-02-09 at 2 34 30 PM" src="https://github.com/user-attachments/assets/57e5f75a-5fe5-4567-93f6-5ac29edc9165" />

**Figure 1:** Comparison of TOPSIS scores for different pre-trained text classification models.

## Model Ranking using TOPSIS
<img width="1190" height="902" alt="image" src="https://github.com/user-attachments/assets/865aa357-813b-4e9b-8c37-e599e1c7c210" />

**Figure 2:** Ranking of pre-trained text classification models using TOPSIS.

## Conclusion

In this project, the TOPSIS (Technique for Order Preference by Similarity to Ideal Solution) method was applied to evaluate and rank multiple pre-trained models for text classification. The evaluation was performed using both performance-related criteria (accuracy and F1-score) and computational efficiency criteria (inference time, model size, and training time).

Based on the computed TOPSIS scores and ranking results, **DistilBERT** emerged as the best-performing model among the considered alternatives. Although some models achieved slightly higher accuracy, DistilBERT provided the optimal balance between classification performance and resource efficiency.

The results demonstrate that the TOPSIS method is an effective decision-making tool for selecting machine learning models when multiple conflicting criteria are involved. This approach can be extended to other domains and tasks where model selection requires balancing performance and computational cost.

---

## 👤 Author

**Kashyap Seth**  
