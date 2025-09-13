## 📊 US Regional Sales Data Analysis

# Analysis of US Regional Sales Data – Data Analytics Project

**🚀 Project Overview**

- This project analyzes US regional sales data to uncover insights about:

- 🏬 Sales performance across different channels

- 🌎 Regional patterns and trends

- 📦 Product performance analysis

- 📅 Seasonal trends and patterns

**📂 Dataset**

- Source: Kaggle - https://www.kaggle.com/datasets/talhabu/us-regional-sales-data

- Records: 7,991 sales transactions

- Time Period: 2018–2021

- Channels: 🏬 In-Store | 💻 Online | 🚚 Distributor | 📦 Wholesale

#### Reproducing data download (Kaggle)
- Install Kaggle CLI (Linux):
  - python3 -m pip install --user kaggle
  - mkdir -p ~/.kaggle
  - Place kaggle.json in ~/.kaggle (from Kaggle account settings)
  - chmod 600 ~/.kaggle/kaggle.json
- Download to data/raw (datasets):
  - kaggle datasets download -d OWNER/DATASET_SLUG -p data/raw --unzip
- If from a competition, use:
  - kaggle competitions download -c COMPETITION_SLUG -p data/raw --unzip

After download, run the cleaning notebook:
- jupyter nbconvert --to notebook --execute notebooks/01_exploratory_analysis_and_ data_cleaning.ipynb

**📁 Project Structure**

- us-regional-sales-analysis/
- ├── data/              # Data files
- ├── notebooks/         # Jupyter notebooks
- ├── src/               # Source code
- ├── reports/           # Generated reports and figures
- └── requirements.txt   # Project dependencies

## 🔑 Key Findings

**🏬 Sales Channel Performance**

- Market Leader: In-Store with 41% share, $30.1M revenue, $8.75M profit, 3,298 orders

- Profitability: Wholesale has the highest ROI (43.2%); Distributor achieves the highest profit per order ($2,813)

- Volatility: Online & In-Store are stable (CV ~21%); Wholesale is most volatile (CV 28.8%)

**📈 Growth & Distribution**

- YoY Growth: Revenue +12.5%, Profit +14.1%, Orders +10.2%

- CAGR (2018–2020): Profit +13.2% > Revenue +11.8% > Orders +9.7%

- Market Concentration: HHI = 3,023 → highly concentrated (dominated by In-Store & Online)

**📦 Product Portfolio**

- Stars (17): Growth engines

- Cash Cows (6): Steady performers

- Question Marks (4): Selective investments

- Dogs (20): Candidates for phase-out

- Top Products: IDs 23, 40, 37, 41, 5 → ~40–45% of total revenue

- Discount Sensitivity: Products 23, 5, 37 yield the highest revenue per discount point

**⏱️ Delivery Performance**

- Avg Processing: 5.6 days | Avg Delivery: 4.3 days | Avg Fulfillment: 5.1 days

- Fast Fulfillment: 63.5% of orders (Target >80%)

- Best Channel: In-Store (Composite Score: 4.2)

- Weakest Channel: Distributor (0.3)

**🏭 Warehouse Insights**

- Top Revenue: WARE-NMK1003 ($23.1M)

- Most Efficient: WARE-NBV1002 (Score: 10.7)

- Least Efficient: WARE-XYS1001 (Score: 0.0)

- Utilization: All warehouses underutilized (<3 daily orders)

**🛠️ Technologies Used**

- 🐍 Python

- 🐼 Pandas

- 📊 Matplotlib & Seaborn

- 📈 Plotly

- 📓 Jupyter Notebooks

**▶️ How to Run**

- Clone this repository

- Install dependencies:

- pip install -r requirements.txt

- Run the Jupyter notebooks in the notebooks/ folder

## 👤 Author

- Abdou Ceesay – Data Analysis Project
