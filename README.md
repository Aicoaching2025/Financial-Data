# KMeans Clustering for Financial Data Segmentation

## 📊 **Project Overview**
This project applies **unsupervised learning** using **KMeans clustering** to segment customers based on financial behavior. By analyzing features like annual income, spending habits, and credit scores, we can identify distinct customer groups, enabling financial institutions to tailor their products more effectively.

## 📝 **Problem Statement**
Financial institutions need to segment their customer base to improve marketing strategies and product offerings. By clustering customers into groups with similar financial behaviors, banks and financial service providers can:
- Offer personalized credit cards or loan options.
- Target high-spending, high-income groups with premium services.
- Identify low-risk and high-risk customer segments.

## 🚀 **Goals**
- Perform **Exploratory Data Analysis (EDA)** to understand customer financial behavior.
- Use **KMeans clustering** to segment customers into distinct groups.
- Visualize and interpret the clusters for actionable business insights.

## 🔍 **Technologies Used**
- Python 3.x  
- Libraries: `numpy`, `pandas`, `matplotlib`, `seaborn`, `scikit-learn`  
- Clustering Algorithm: **KMeans** from `scikit-learn`  

## 📂 **Project Structure**
```
kmeans-finance-segmentation/
├── data/
│   └── segmented_customers.csv        # Final dataset with cluster labels
├── notebooks/
│   └── kmeans_clustering_analysis.ipynb  # EDA, modeling, and visualization
├── src/
│   └── data_generation.py            # Script for generating synthetic data
│   └── clustering_model.py           # Code for KMeans clustering and evaluation
├── requirements.txt                  # Required Python libraries
└── README.md                         # Project overview and instructions
```

## 🗂️ **Dataset Description**
The generated synthetic dataset contains the following features:
- **Annual Income (k$):** Income range from 20k to 150k.
- **Spending Score (1-100):** Indicator of spending behavior.
- **Credit Score (300-850):** Customer's creditworthiness.
- **Cluster:** Assigned customer segment from KMeans clustering.

## 🛠️ **Installation & Setup**
1. **Clone the repository:**
```bash
git clone https://github.com/your-username/kmeans-finance-segmentation.git
cd kmeans-finance-segmentation
```
2. **Create a virtual environment (optional):**
```bash
python -m venv env
source env/bin/activate  # For Unix/macOS
# or
env\Scripts\activate    # For Windows
```
3. **Install dependencies:**
```bash
pip install -r requirements.txt
```
4. **Run the analysis notebook:**
```bash
jupyter notebook notebooks/kmeans_clustering_analysis.ipynb
```

## 🧮 **Methods & Steps**
### 1. **Data Generation & Exploration**
- Generate synthetic financial data (income, spending, credit score).
- Visualize relationships between features using scatter plots and pairplots.

### 2. **Preprocessing**
- Scale features using `StandardScaler` for fair distance measurements.
- Check for outliers and handle missing values if needed.

### 3. **Choosing Optimal Clusters**
- **Elbow Method:** Analyze WCSS to determine the appropriate number of clusters.
- **Silhouette Score:** Evaluate cluster quality.

### 4. **Modeling with KMeans**
- Train KMeans with the selected number of clusters.
- Assign cluster labels to the dataset.

### 5. **Visualization & Interpretation**
- Plot clusters with different colors to understand segmentation.
- Analyze cluster centers to describe typical customer profiles.

### 6. **Results & Business Insights**
| Cluster | Annual Income (k$) | Spending Score | Credit Score | Description |
|---------|-------------------|----------------|--------------|-------------|
| 0       | 120k               | 80             | 750          | High-income, high-spenders |
| 1       | 60k                | 40             | 650          | Middle-income, moderate spenders |
| 2       | 30k                | 70             | 600          | Low-income, high spenders |
| 3       | 80k                | 20             | 700          | High-income, low spenders |

## 📈 **Sample Visualization**
The scatter plot below shows customer segments based on annual income and spending score:

![Cluster Visualization](assets/cluster_visualization.png)

## 🚀 **How to Contribute**
1. Fork the repository.
2. Create a feature branch: `git checkout -b feature/your-feature-name`.
3. Commit your changes: `git commit -m "Add new feature"`.
4. Push to the branch: `git push origin feature/your-feature-name`.
5. Open a pull request.

## 📬 **Contact**
For questions or suggestions, feel free to reach out:  
📧 your.email@example.com  
🌐 [Your LinkedIn](https://www.linkedin.com/in/your-profile/)  

---

## 💡 **Future Improvements**
- Add real-world financial datasets for improved modeling.
- Incorporate other clustering methods (DBSCAN, Hierarchical Clustering).
- Deploy the solution as an interactive dashboard.

---
## 🏁 **Conclusion**
###This project demonstrates the power of **unsupervised learning** through **KMeans clustering** to segment customers based on financial behaviors such as income, spending, and credit scores. By generating synthetic data and applying clustering techniques, we successfully identified distinct customer segments that can guide financial institutions in personalizing their services and improving marketing strategies. 

## 📊 **Specific Insights:**
- **Cluster 0 (High-income, high-spenders):** Represents affluent customers who frequently spend and may be ideal for premium credit cards or exclusive financial services. 
- **Cluster 1 (Middle-income, moderate spenders):** Stable earners with average spending patterns, suitable for standard financial products with occasional promotions. 
- **Cluster 2 (Low-income, high spenders):** Customers with lower income but higher spending habits, potentially high-risk for credit but valuable for targeted budgeting services. 
- **Cluster 3 (High-income, low spenders):** Wealthy but frugal clients who may be interested in investment opportunities or high-yield savings products. 

These insights allow financial institutions to craft targeted marketing strategies, optimize product offerings, and improve customer retention by understanding the unique behaviors of each segment. This project not only showcases how machine learning can solve real-world business problems but also provides a strong foundation for further exploration with real datasets and advanced clustering methods.

## 🗝️ **Key Findings for Stakeholders:**
1. **Four Distinct Customer Segments Identified:**  
   - High-income, high-spenders (Cluster 0): Prime candidates for premium financial products and exclusive services.
   - Middle-income, moderate spenders (Cluster 1): Ideal for standard offerings with value-driven incentives.
   - Low-income, high spenders (Cluster 2): Potentially high-risk clients requiring targeted financial literacy programs or budget management tools.
   - High-income, low spenders (Cluster 3): Suitable for investment products and long-term financial planning services.

2. **Significant Variation in Spending Habits:**  
   Customers with similar incomes exhibit vastly different spending patterns, emphasizing the need for behavioral-based segmentation rather than relying solely on income levels.

3. **Credit Score Correlation:**  
   Clusters with higher credit scores align with higher income groups, highlighting lower default risks and better creditworthiness for certain segments.

4. **Actionable Business Opportunities:**  
   - Design personalized marketing campaigns targeting high-spending segments.
   - Develop new financial products for underserved groups, particularly low-income, high spenders.
   - Improve customer retention by offering tailored rewards and promotions.

5. **Data-Driven Strategy Advantages:**  
   Utilizing this segmentation enables better allocation of marketing resources, improved customer satisfaction, and increased ROI through targeted service offerings.

These key findings provide a clear roadmap for strategic decision-making, helping stakeholders prioritize customer engagement efforts and enhance overall business performance.



🚀 **Let’s use data to make smarter financial decisions!**

