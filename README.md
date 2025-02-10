# Movie Recommendation System

## Overview
This repository contains various implementations of a **Movie Recommendation System**, utilizing multiple machine learning techniques including **Collaborative Filtering, Content-Based Filtering, Deep Learning, and Hybrid Methods**.

## Features
- **User-Based & Item-Based Collaborative Filtering** (KNN-based algorithms)
- **Matrix Factorization** (Singular Value Decomposition - SVD)
- **Deep Learning-Based Recommendations** (RBM, AutoRec)
- **Hybrid Recommendation System** (Combining multiple models)
- **Scalability using Apache Spark**

## Repository Structure
```
MovieRecommendationSystem/
│── ContentBased/
│   ├── ContentKNNAlgorithm.py
│   ├── ContentRecs.py
│   ├── EvaluatedAlgorithm.py
│   ├── EvaluationData.py
│   ├── Evaluator.py
│   ├── MovieLens.py
│   ├── RecommenderMetrics.py
│
│── CollaborativeFiltering/
│   ├── EvaluateUserCF.py
│   ├── EvaluatedAlgorithm.py
│   ├── EvaluationData.py
│   ├── Evaluator.py
│   ├── KNNBakeOff.py
│   ├── MovieLens.py
│   ├── SimpleItemCF.py
│   ├── SimpleUserCF.py
│
│── DeepLearning/
│   ├── AutoRec.py
│   ├── AutoRecAlgorithm.py
│   ├── AutoRecBakeOff.py
│   ├── RBM.py
│   ├── RBMAlgorithm.py
│   ├── RBMBakeOff.py
│   ├── RBMTuning.py
│   ├── MovieLens.py
│   ├── Evaluator.py
│
│── Hybrid/
│   ├── HybridAlgorithm.py
│   ├── HybridTest.py
│   ├── MovieLens.py
│   ├── RBM.py
│   ├── RBMAlgorithm.py
│   ├── ContentKNNAlgorithm.py
│
│── MatrixFactorization/
│   ├── SVDBakeOff.py
│   ├── SVDTuning.py
│   ├── Evaluator.py
│   ├── MovieLens.py
│
│── ScalingUp/
│   ├── SparkALS.py
│   ├── SparkALS-20m.py
│   ├── winutils.exe
│   ├── MovieLens.py
```

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/kartiknarang04/MovieRecommendationSystem.git
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

## Usage
Run the appropriate script depending on the recommendation model:
- **Content-Based Filtering:**
  ```sh
  python ContentBased/ContentKNNAlgorithm.py
  ```
- **Collaborative Filtering:**
  ```sh
  python CollaborativeFiltering/KNNBakeOff.py
  ```
- **Deep Learning-Based Recommendation:**
  ```sh
  python DeepLearning/AutoRec.py
  ```
- **Hybrid Recommendation:**
  ```sh
  python Hybrid/HybridAlgorithm.py
  ```
- **Matrix Factorization (SVD):**
  ```sh
  python MatrixFactorization/SVDBakeOff.py
  ```
- **Scalability with Spark:**
  ```sh
  python ScalingUp/SparkALS.py
  ```

## Dataset
The system uses the **MovieLens Dataset**. You can download it from [MovieLens](https://grouplens.org/datasets/movielens/).

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributors
- **Kartik Narang** ([@kartiknarang04](https://github.com/kartiknarang04))

## Acknowledgments
- **MovieLens Dataset** provided by GroupLens Research.
- **Surprise Library** for collaborative filtering models.
- **Apache Spark** for large-scale recommendation systems.

