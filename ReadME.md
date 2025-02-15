## Supply Chain Data Processing & Predictive Analysis

This project focuses on handling supply chain data, inserting it into MongoDB, and performing predictive analysis using machine learning techniques.

### 📌 Project Components

1. **Data Insertion (`insert_data_mongo.ipynb`)**  
   - Reads supply chain data from a CSV file.  
   - Inserts the data into MongoDB under the `supply_chain_data` collection.  

2. **Predictive Analysis (`predictive_analysis_supply_chain.ipynb`)**  
   - Loads supply chain data from MongoDB.  
   - Uses Apache Spark for data preprocessing.  
   - Trains a **Random Forest Regressor** to predict inventory pricing.  
   - Stores predictions in MongoDB under the `prediction_data` collection.  

### ⚙️ Tech Stack

- **MongoDB** (for data storage)  
- **Apache Spark** (for predictive analysis)  
- **Python Libraries:**
  - `pymongo` (for MongoDB interaction)
  - `pyspark` (for machine learning and data processing)
  - `pandas` (for handling CSV data)

### 🚀 Setup Instructions

1. **Install Dependencies**  
   ```sh
   pip install pymongo pyspark pandas
   ```

2. **Insert Data into MongoDB**  
   - Run `insert_data_mongo.ipynb` to load supply chain data into MongoDB.

3. **Run Predictive Analysis**  
   - Run `predictive_analysis_supply_chain.ipynb` to train the model and store predictions.

### 📈 Predictive Analysis Workflow

- Uses **Random Forest Regression** for price prediction.
- Features: `Price` and `Stock Levels`.
- Trained model predicts pricing trends in supply chain management.

### 📊 Output

- Predictions are stored in MongoDB for further business insights.