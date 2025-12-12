# **Breast Cancer Diagnosis Prediction using K-Nearest Neighbors (KNN) & K-Means Clustering**

This project classifies breast cancer tumors as **Malignant (M)** or **Benign (B)** using two machine learning techniques:

* **K-Nearest Neighbors (KNN)** – Supervised Classification
* **K-Means Clustering** – Unsupervised Clustering

The dataset used is the **Breast Cancer Wisconsin Diagnostic Dataset**.

---

## **📌 Objectives**

1. Encode the diagnosis column:

   * **M → 1**, **B → 0**
2. Remove unnecessary columns:

   * `id`, `Unnamed: 32`
3. Normalize numerical features using **Min-Max Scaling**
4. Split dataset into:

   * **80% Training**
   * **20% Testing**
5. Apply **K-Means (k = 2)** to observe natural clustering of tumor types.
6. Train a **KNN Classifier (k = 5)**.
7. Evaluate the model using:

   * Accuracy
   * Precision
   * Recall
   * F1-Score

---

## **📂 Project Structure**

```
BreastCancerPrediction/
│
├── data.csv
├── KNN_KMeans_BreastCancer.ipynb
├── README.md
```

---

## **⚙️ Requirements**

Install required libraries (Colab already includes them):

```bash
pip install numpy pandas scikit-learn
```

---

## **🧪 Methods Used**

### **1. Data Preprocessing**

* Dropping non-useful columns
* Encoding categorical diagnosis values
* Feature normalization using MinMaxScaler

### **2. K-Means Clustering**

Used to group data into **2 clusters**:

* Unsupervised grouping of patients
* Helps visualize natural separation in data

### **3. KNN Classification**

* Supervised learning algorithm
* Uses **k = 5** nearest neighbors
* Predicts tumor type based on similarity

---

## **📊 Evaluation Metrics**

The classifier is evaluated using:

* **Accuracy** – Overall correctness
* **Precision** – Correctly identified malignant cases
* **Recall** – Ability to detect malignant cases
* **F1-Score** – Balance between precision & recall

These metrics help determine overall model performance.

---

## **▶️ How to Run in Google Colab**

1. Upload `data.csv` to Colab
2. Copy the single-cell code into a new notebook
3. Run all sub-cells
4. View model evaluation results

---

## **📝 Expected Output**

* Cluster assignments from K-means
* KNN model metrics:

  * Accuracy
  * Precision
  * Recall
  * F1-score
* Classification report

---

## **✔️ Conclusion**

This project demonstrates how combining **supervised and unsupervised** methods helps understand breast cancer data better:

* **K-Means** reveals how well malignant/benign data naturally clusters
* **KNN** provides strong performance in predicting cancer diagnosis

This workflow is widely used in medical data science and diagnostic support systems.


