# Predatory Activity Index for Ireland

[License: MIT](https://opensource.org/licenses/MIT)  
[Python 3.9+](https://www.python.org/downloads/)  
[Status: Prototype]()

---

## 📌 **Overview**

The **Predatory Activity Index (PAI) for Ireland** is a **real-time, data-driven tool** designed to measure, monitor, and mitigate predatory behaviors impacting **individuals, families, businesses, and institutions** in Ireland. Developed by **Transparency-X**, this index aggregates data from public and private sources to provide actionable insights into scams, fraud, cybercrime, workplace exploitation, and other predatory activities.

### **Purpose**

- **Track**: Monitor predatory activity trends over time.
- **Detect**: Identify spikes or emerging threats in real time.
- **Prevent**: Empower stakeholders (government, businesses, consumers) to take proactive measures.
- **Monetize**: Generate revenue through subscriptions, API access, and partnerships.

### **Why Ireland?**

Ireland’s strong digital infrastructure, open data initiatives, and active regulatory bodies (e.g., CCPC, Gardaí, Central Bank) make it an ideal testbed for this index. The prototype can later be scaled to other countries.

---

## 🚀 **Features**

### **Core Features**

✅ **Multi-Category Tracking**: Monitors financial scams, cybercrime, consumer complaints, workplace exploitation, and elder abuse.  
✅ **Real-Time Data Aggregation**: Combines data from public sources (e.g., CCPC, Gardaí) and private partnerships (e.g., banks, telcos).  
✅ **Normalized Scoring**: Each category is scored on a 0–100 scale for comparability.  
✅ **Weighted Composite Index**: Aggregates category scores into a single **Predatory Activity Index (PAI)**.  
✅ **Interactive Dashboard**: Visualizes trends, hotspots, and alerts (prototype available).  
✅ **Alert System**: Flags spikes in predatory activity (e.g., "Cybercrime score > 80").

### **Prototype Features**

- Mock dataset simulating real-world predatory activity (Jan–May 2026).
- Composite index calculation with customizable weights.
- Visualization of trends (see [Prototype Output](#prototype-output)).

### **Planned Features**

🔜 **Live Data Integration**: Replace mock data with real-time feeds from CCPC, Gardaí, and other sources.  
🔜 **Geospatial Analysis**: Map predatory activity by county/region.  
🔜 **Predictive Modeling**: Forecast trends using machine learning (e.g., Prophet, ARIMA).  
🔜 **API Access**: Allow third-party developers to integrate PAI data into their systems.  
🔜 **User Reporting Portal**: Enable public reporting of scams/exploitation.  
🔜 **Custom Reports**: Generate tailored reports for specific sectors (e.g., finance, healthcare).

---

## 📂 **Project Structure**

```
predatory-activity-index-ireland/
├── README.md                          # Project overview (this file)
├── docs/
│   ├── OVERVIEW.md                    # Detailed project overview
│   ├── FEATURES.md                    # Feature list and descriptions
│   └── ROADMAP.md                     # Development roadmap
├── data/
│   ├── mock/                          # Mock datasets for prototyping
│   │   ├── financial_scams.csv        # Mock financial scam data
│   │   ├── cybercrime.csv             # Mock cybercrime data
│   │   ├── consumer_complaints.csv    # Mock consumer complaint data
│   │   ├── workplace_exploitation.csv # Mock workplace exploitation data
│   │   └── elder_abuse.csv            # Mock elder abuse data
│   └── real/                          # Real data (to be populated)
│       ├── ccpc/                      # CCPC scam alerts
│       ├── garda/                     # Garda cybercrime reports
│       └── central_bank/              # Central Bank fraud data
├── outputs/
│   ├── visualizations/                # Generated charts and graphs
│   │   └── ireland_predatory_activity_index_prototype.png  # Prototype visualization
│   └── reports/                       # Analysis reports
│       └── prototype_analysis.md      # Insights from prototype data
├── src/
│   ├── data_collection/              # Scripts to fetch/clean data
│   │   ├── scrape_ccpc.py             # Scrape CCPC scam alerts
│   │   ├── fetch_garda_data.py        # Fetch Garda cybercrime stats
│   │   └── process_data.py            # Clean and normalize data
│   ├── processing/                    # Index calculation logic
│   │   ├── calculate_scores.py        # Normalize and weight scores
│   │   └── composite_index.py         # Generate composite PAI
│   └── visualization/                 # Dashboard and plotting scripts
│       ├── plot_trends.py             # Generate time-series plots
│       └── dashboard.py               # Interactive dashboard (e.g., Plotly Dash)
├── .github/
│   └── workflows/                     # GitHub Actions for CI/CD
│       └── update_data.yml            # Automate data updates
├── LICENSE                            # MIT License
└── requirements.txt                  # Python dependencies
```

---

## 🛠️ **Installation**

### **Prerequisites**

- Python 3.9+
- Git
- Required libraries (see `requirements.txt`)

### **Setup**

1. Clone the repository:
  ```bash
   git clone https://github.com/transparency-x/predatory-activity-index-ireland.git
   cd predatory-activity-index-ireland
  ```
2. Install dependencies:
  ```bash
   pip install -r requirements.txt
  ```
3. Run the prototype:
  ```bash
   python src/processing/composite_index.py
  ```

---

## 📊 **Prototype Output**

### **Sample Visualization**

A prototype of the **Ireland Predatory Activity Index** (Jan–May 2026) is available:

- **Composite Index**: Aggregated score (0–100) of all predatory activities.
- **Category Trends**: Individual scores for financial scams, cybercrime, consumer complaints, workplace exploitation, and elder abuse.

Ireland Predatory Activity Index Prototype

> **Note**: This visualization uses **mock data** to simulate real-world trends. Replace with live data for production.

### **Sample Data**

Mock datasets are provided in `data/mock/`. Example:

- `financial_scams.csv`: Daily reports of scams (phishing, romance scams, etc.).
- `cybercrime.csv`: Daily cybercrime incidents (ransomware, hacking, etc.).

---

## 📈 **Roadmap**

### **Phase 1: Prototype (Q2 2026)**

- Define index methodology and categories.
- Generate mock datasets for testing.
- Build composite index calculation logic.
- Create prototype visualization.
- Validate methodology with stakeholders (CCPC, Gardaí).

### **Phase 2: MVP (Q3–Q4 2026)**

- Integrate **real data** from CCPC, Gardaí, and Central Bank.
- Develop **ETL pipeline** for automated data collection.
- Launch **static dashboard** (monthly updates).
- Secure **pilot partnerships** (e.g., 1–2 banks or NGOs).

### **Phase 3: Live Index (2027)**

- Deploy **real-time dashboard** (daily updates).
- Add **geospatial analysis** (county-level trends).
- Implement **API access** for third-party integrations.
- Launch **user reporting portal** for public contributions.
- Expand to **EU/UK markets** (e.g., "European Predatory Activity Index").

### **Phase 4: Scaling (2028+)**

- Add **predictive modeling** (forecast trends).
- Introduce **custom reports** for sectors (e.g., finance, healthcare).
- Monetize via **subscriptions, sponsorships, and grants**.
- Partner with **global organizations** (e.g., Transparency International, Europol).

---

## 🤝 **Contributing**

We welcome contributions! Please read our [Contributing Guidelines](CONTRIBUTING.md) for details on how to get involved.

---

## 📄 **License**

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

## 📬 **Contact**

For questions or collaborations, contact:

- **Declan** (Transparency-X): [declan@transparency-x.com](mailto:declan@transparency-x.com)
- **Project Repository**: [github.com/transparency-x/predatory-activity-index-ireland](https://github.com/transparency-x/predatory-activity-index-ireland)

---

## 🙏 **Acknowledgments**

- **Data Sources**: CCPC, Gardaí, Central Bank of Ireland, HSE, WRC.
- **Inspiration**: Transparency International’s Corruption Perceptions Index, UK’s Fraud Risk Index.
- **Tools**: Python, Pandas, Matplotlib, Plotly Dash, BeautifulSoup.
