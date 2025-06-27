# Which Clusters Better? 🧠 Deep Embedded Clustering (DEC) vs EFCM

## Project summary
This project compares two clustering approaches, EFCM (Enhanced Fuzzy C-Means) and DEC (Deep Embedded Clustering), for unsupervised topic discovery in user-generated text.
The goal is to evaluate which method produces more coherent topics when applied to review data embedded using BERT. 
DEC, which combines deep learning and clustering in a unified framework, is expected to outperform traditional fuzzy methods due to its ability to learn meaningful feature representations.

## Outcome summary
<p align="center">
  <img src="https://github.com/user-attachments/assets/47051cfa-8953-4b2f-8cac-9bf765d0a634" width="400"/>
</p>

The experiment tested topic coherence across 1–10 clusters using TC-W2V (Topic Coherence with Word2Vec). 
DEC consistently outperformed EFCM, peaking at 0.23428 with 4 clusters.

|![image](https://github.com/user-attachments/assets/56190e78-b9bf-4d7f-b2f8-1e2eeb5dcc3e)|![image](https://github.com/user-attachments/assets/8afc44cf-aa6d-4814-b992-f9d9805fb403)|
|:--:|:--:|
| DEC Clusters Result | EFCM Clusters Result |

DEC produced tighter, more clearly separated clusters, thanks to its built-in parameter optimization during training. 
EFCM showed more overlapping clusters, as it lacks a parameter optimization phase, leading to less distinct topic boundaries.
While EFCM was competitive at some points, its coherence scores were less stable across different topic numbers.

## Recommendation
DEC-based clustering model can be integrated into intelligent dashboards for businesses to extract trending topics from user reviews, enabling faster, data-driven decision-making.

## Technologies used
`Python` `Transformers (HuggingFace)` `BERT` `DEC` `google-play-scraper` `scikit-learn` `pandas` `numpy` `matplotlib` `seaborn`
