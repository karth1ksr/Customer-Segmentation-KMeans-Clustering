# Project: Customer Segmentation Using KMeans Clustering

## Objective
To segment customers into distinct behavioral groups based on their purchasing patterns using the KMeans clustering algorithm. This enables targeted marketing and customer engagement strategies.

## Dataset Description (`OnlineRetail.csv`)
Contains transactional data of a UK-based online retail store:
- `InvoiceNo`: Unique ID per transaction
- `StockCode`: Product code
- `Description`: Product name
- `Quantity`: Number of items purchased
- `InvoiceDate`: Timestamp of transaction
- `UnitPrice`: Price per item
- `CustomerID`: Unique identifier for each customer
- `Country`: Customer’s location

## Key Steps in Notebook
1. Load and clean the dataset
   - Handle missing Customer IDs and duplicates
   - Remove cancellations (negative quantity invoices)
2. Perform EDA
3. Use **Elbow Method** and **Silhouette Score** to determine optimal number of clusters
4. Apply KMeans clustering to segment customers
5. Visualize clusters in 2D using PCA or t-SNE
6. Export segmented customer data

## Requirements
- Python 3.8+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

To install all dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Folder Structure
<pre><code> 
```bash
Customer-Segmentation-KMeans-Clustering/
├── data/ # Dataset files
├── notebooks/ # Jupyter notebooks for EDA and model training
├── preprocessed_segmentation.pkl/ # Preprocessed pkl file for training the model
└── README.md # Project documentation
```
</code></pre>

## How to Run
*  Open preprocessing_segmentation.ipynb from the notebooks/ in Jupyter Notebook or VS Code

*  Ensure OnlineRetail.csv is present in the same directory

*  Run all cells sequentially to clean and process the data

*  Load the k_means_cs.ipynb from the notebooks/ in Jupyter Notebook or VS Code

*  Ensure preprocessed_segmentation.pkl is in the same directory

*  Run all the cells to apply clustering and view segment patterns

## Output
*  Clustered customer data

*  Visualizations of cluster centers and distributions

