# **Emerging Research Trends Clustering**

## **📌 Project Overview**
This project aims to **identify and track emerging research trends** by clustering research papers from arXiv. Using **Deep Embedded Clustering (DEC) and Time-Series Analysis**, we can analyze how topics evolve over time and discover **new interdisciplinary research areas**.

## **🎯 Objectives**
- Fetch research papers from **arXiv API** (2015-2025).
- Extract **semantic embeddings** using **BERT/TF-IDF**.
- Cluster papers into **meaningful research topics** using **DEC/HDBSCAN**.
- Track **how topics evolve over time** to detect **emerging trends**.
- Visualize trends using **t-SNE, UMAP, and time-series graphs**.

## **📂 Project Structure**
```
📂 Emerging_Research_Trends_Clustering
│── 📁 data
│   ├── research_papers_2015_2025.csv  # Collected paper data
│   ├── embeddings.npy  # Embeddings for clustering
│── 📁 models
│   ├── clustering_DEC.pkl  # Trained clustering model
│   ├── topic_embeddings_BERT.pkl  # Precomputed embeddings
│── 📂 notebooks
│   ├── 1_data_collection.ipynb  # Fetching data from arXiv
│   ├── 2_text_preprocessing.ipynb  # Cleaning & embedding text
│   ├── 3_clustering.ipynb  # Clustering papers into topics
│   ├── 4_trend_analysis.ipynb  # Analyzing topic growth
│   ├── 5_visualization.ipynb  # Generating visual reports
│── 📂 streamlit_dashboard
│   ├── app.py  # Interactive dashboard to explore trends
│── requirements.txt  # Python dependencies
│── README.md  # Project documentation
```

## **📊 How It Works**
1. **Data Collection:** Fetch papers from arXiv API with metadata (title, abstract, keywords, year).
2. **Text Embedding:** Convert text into **BERT or TF-IDF embeddings**.
3. **Clustering:** Use **Deep Embedded Clustering (DEC) or HDBSCAN** to group papers into research topics.
4. **Trend Analysis:** Track cluster size and growth over time to identify emerging trends.
5. **Visualization:** Use **t-SNE, UMAP, and time-series graphs** to explore research evolution.

## **🔧 Setup Instructions**
### **1️⃣ Install Dependencies**
```bash
pip install -r requirements.txt
```

### **2️⃣ Fetch Data from arXiv**
Run the data collection script to download research papers.
```bash
python notebooks/1_data_collection.ipynb
```

### **3️⃣ Preprocess Text and Generate Embeddings**
```bash
python notebooks/2_text_preprocessing.ipynb
```

### **4️⃣ Train Clustering Model**
```bash
python notebooks/3_clustering.ipynb
```

### **5️⃣ Run Visualization Dashboard**
```bash
cd streamlit_dashboard
streamlit run app.py
```

## **📈 Expected Results**
- **Clusters of research topics** with keywords for labeling.
- **Time-series graphs** showing **emerging vs. declining fields**.
- **Interactive exploration** of research trends.

## **🚀 Future Enhancements**
- **Integrate Citation Graphs** using GNNs to analyze **influence between topics**.
- **Expand to Google Scholar & Semantic Scholar** for a broader dataset.
- **Real-time trend updates** for new research papers.

---
## **👨‍💻 Contributors & Contact**
If you have any questions or want to contribute, feel free to reach out!