# Predatory Activity Index for Ireland: Features

---

## 📋 **Feature Overview**

The **Predatory Activity Index (PAI) for Ireland** is designed to be a **comprehensive, real-time, and actionable** tool for tracking predatory behaviors. Below is a detailed list of its **current, planned, and potential features**, categorized by functionality.

---

## ✅ **Core Features (Prototype Phase)**

### **1. Data Aggregation & Processing**


| **Feature**              | **Description**                                                                                                      | **Status** | **Data Sources**                    |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------- | ---------- | ----------------------------------- |
| Multi-Category Tracking  | Tracks **5 core categories**: Financial Scams, Cybercrime, Consumer Complaints, Workplace Exploitation, Elder Abuse. | ✅ Complete | Mock data (CCPC, Gardaí, WRC, HSE)  |
| Daily Data Rollup        | Aggregates data into **daily scores** for trend analysis.                                                            | ✅ Complete | Mock datasets                       |
| Normalization            | Scales all metrics to a **0–100 range** for comparability.                                                           | ✅ Complete | Custom Python scripts               |
| Weighted Composite Index | Calculates a **single PAI score** using customizable weights (e.g., Financial Scams = 30%).                          | ✅ Complete | `src/processing/composite_index.py` |
| Mock Data Generation     | Simulates **realistic predatory activity trends** for prototyping.                                                   | ✅ Complete | `data/mock/`                        |


### **2. Visualization & Reporting**


| **Feature**               | **Description**                                                           | **Status** | **Output**                 |
| ------------------------- | ------------------------------------------------------------------------- | ---------- | -------------------------- |
| Time-Series Plots         | Generates **line charts** of PAI and category scores over time.           | ✅ Complete | `outputs/visualizations/`  |
| Composite Index Dashboard | Displays the **PAI score**, category trends, and alerts in a single view. | ✅ Complete | Prototype PNG (see README) |
| Data Export               | Exports **CSV/Excel reports** for further analysis.                       | ✅ Complete | `outputs/reports/`         |


---

## 🚀 **Planned Features (MVP Phase)**

### **1. Real-Time Data Integration**


| **Feature**                | **Description**                                                                      | **Priority** | **Data Sources**                                 |
| -------------------------- | ------------------------------------------------------------------------------------ | ------------ | ------------------------------------------------ |
| CCPC Scam Alerts           | Pulls **live scam reports** from the Competition and Consumer Protection Commission. | High         | [CCPC API/Website](https://www.ccpc.ie/)         |
| Garda Cybercrime Stats     | Integrates **cybercrime incident data** from An Garda Síochána.                      | High         | [Garda Crime Stats](https://www.garda.ie/)       |
| Central Bank Fraud Data    | Incorporates **financial fraud reports** from the Central Bank of Ireland.           | High         | [Central Bank Data](https://www.centralbank.ie/) |
| Revenue Commissioners Data | Adds **tax evasion and VAT fraud** metrics.                                          | Medium       | [Revenue.ie](https://www.revenue.ie/)            |
| HSE Elder Abuse Reports    | Tracks **elder abuse cases** from Health Service Executive.                          | Medium       | [HSE Safeguarding](https://www.hse.ie/)          |
| WRC Workplace Cases        | Monitors **workplace exploitation** via Workplace Relations Commission.              | Medium       | [WRC Reports](https://www.wrc.ie/)               |


### **2. Enhanced Analytics**


| **Feature**             | **Description**                                                                   | **Priority** | **Tools/Libraries**       |
| ----------------------- | --------------------------------------------------------------------------------- | ------------ | ------------------------- |
| Geospatial Mapping      | Maps predatory activity by **county/region** (e.g., Dublin vs. Cork).             | High         | Folium, Plotly, QGIS      |
| Anomaly Detection       | Flags **unusual spikes** in predatory activity (e.g., sudden rise in ransomware). | High         | PyOD, Scikit-learn        |
| Severity Scoring        | Assigns **risk levels** (Low/Medium/High) to incidents.                           | Medium       | Custom logic              |
| Sector-Specific Reports | Generates **tailored reports** for finance, healthcare, retail, etc.              | Medium       | Pandas, Jupyter Notebooks |


### **3. User Engagement**


| **Feature**             | **Description**                                                                        | **Priority** | **Implementation**        |
| ----------------------- | -------------------------------------------------------------------------------------- | ------------ | ------------------------- |
| Public Reporting Portal | Allows **citizens to report scams/exploitation** via a web form.                       | High         | Flask/Django + PostgreSQL |
| Email Alerts            | Sends **automated alerts** to subscribers when PAI spikes.                             | High         | SMTP, Twilio              |
| API Access              | Provides **REST API** for third-party integrations (e.g., banks, cybersecurity firms). | High         | FastAPI, Flask            |
| Mobile App              | Offers a **mobile-friendly dashboard** for on-the-go access.                           | Low          | React Native, Flutter     |


---

## 🌟 **Advanced Features (Scaling Phase)**

### **1. Predictive Analytics**


| **Feature**                 | **Description**                                                              | **Priority** | **Tools/Techniques**                      |
| --------------------------- | ---------------------------------------------------------------------------- | ------------ | ----------------------------------------- |
| Trend Forecasting           | Predicts **future PAI trends** using historical data.                        | High         | Prophet, ARIMA, LSTM                      |
| Risk Scoring for Businesses | Assigns **predatory risk scores** to businesses based on sector/location.    | High         | Machine Learning (XGBoost, Random Forest) |
| Early Warning System        | Identifies **emerging threats** (e.g., new scam types) before they escalate. | Medium       | NLP (spaCy), Anomaly Detection            |


### **2. Integration & Automation**


| **Feature**                 | **Description**                                                                      | **Priority** | **Tools**                |
| --------------------------- | ------------------------------------------------------------------------------------ | ------------ | ------------------------ |
| Bank Transaction Monitoring | Integrates with **bank APIs** to flag suspicious transactions in real time.          | High         | Plaid, Open Banking APIs |
| Government Dashboard        | Provides a **custom dashboard** for regulators (e.g., CCPC, Gardaí).                 | High         | Plotly Dash, Tableau     |
| Automated Workflows         | Triggers **actions** based on PAI scores (e.g., freeze transactions, notify Gardaí). | Medium       | Zapier, Airflow          |
| Blockchain Verification     | Stores **PAI data on a blockchain** for transparency and immutability.               | Low          | Ethereum, Hyperledger    |


### **3. Expansion & Customization**


| **Feature**             | **Description**                                                                                 | **Priority** | **Scope**                           |
| ----------------------- | ----------------------------------------------------------------------------------------------- | ------------ | ----------------------------------- |
| EU-Wide Index           | Expands the PAI to **other European countries**.                                                | High         | EU Open Data Portal                 |
| Sector-Specific Indices | Creates **custom indices** for finance, healthcare, real estate, etc.                           | Medium       | Domain-specific data sources        |
| Global Index            | Develops a **Global Predatory Activity Index** in partnership with international organizations. | Low          | Transparency International, Europol |
| White-Label Solutions   | Offers **custom-branded PAI dashboards** for businesses/NGOs.                                   | Medium       | React, Plotly Dash                  |


---

## 🔧 **Technical Features**

### **1. Backend**

- **Language**: Python 3.9+
- **Libraries**: Pandas, NumPy, Scikit-learn, PyOD, Requests, BeautifulSoup
- **ETL Pipeline**: Apache Airflow, Apache NiFi
- **Database**: PostgreSQL (relational), MongoDB (NoSQL)
- **API**: FastAPI, Flask

### **2. Frontend**

- **Dashboard**: Plotly Dash, Streamlit
- **Geospatial**: Folium, Leaflet
- **Mobile**: React Native (future)

### **3. DevOps**

- **Version Control**: Git/GitHub
- **CI/CD**: GitHub Actions
- **Hosting**: AWS (EC2, S3), Google Cloud, or Heroku
- **Monitoring**: Prometheus, Grafana

---

## 📊 **Feature Roadmap**

### **Phase 1: Prototype (Q2 2026)**

- Define index methodology and categories.
- Generate mock datasets.
- Build composite index calculation.
- Create prototype visualization.
- Validate with stakeholders.

### **Phase 2: MVP (Q3–Q4 2026)**

- Integrate real data from CCPC, Gardaí, Central Bank.
- Develop ETL pipeline for automated data collection.
- Launch static dashboard (monthly updates).
- Secure pilot partnerships (e.g., banks, NGOs).
- Add geospatial mapping.
- Implement email alerts.

### **Phase 3: Live Index (2027)**

- Deploy real-time dashboard (daily updates).
- Add predictive modeling (Prophet, ARIMA).
- Launch API access for third parties.
- Develop public reporting portal.
- Expand to EU/UK markets.

### **Phase 4: Scaling (2028+)**

- Introduce blockchain verification.
- Add sector-specific indices.
- Launch mobile app.
- Monetize via subscriptions, API fees, sponsorships.

---

## 💡 **Potential Future Features**


| **Feature**                   | **Description**                                                              | **Feasibility** | **Impact**                |
| ----------------------------- | ---------------------------------------------------------------------------- | --------------- | ------------------------- |
| AI-Powered Chatbot            | Answers user questions about predatory activity in natural language.         | Medium          | High (user engagement)    |
| Voice Alerts                  | Sends **voice call alerts** to vulnerable populations (e.g., elderly).       | Low             | High (accessibility)      |
| Augmented Reality (AR)        | Overlays **PAI data on AR maps** (e.g., "Avoid this area – high scam risk"). | Low             | Medium (innovation)       |
| Gamification                  | Rewards users for **reporting scams** or **completing safety training**.     | Medium          | Medium (engagement)       |
| Partnership with Social Media | Integrates with **Twitter/Facebook** to detect scam trends in real time.     | High            | High (real-time insights) |


---

## 📌 **How to Contribute**

Interested in helping develop these features?

1. **Fork the repository** on GitHub.
2. **Pick an open issue** from the [Issues](https://github.com/transparency-x/predatory-activity-index-ireland/issues) tab.
3. **Submit a pull request** with your changes.
4. **Join the discussion** in our [Discussions](https://github.com/transparency-x/predatory-activity-index-ireland/discussions) tab.

---

## 📬 **Feedback**

Have a feature request or idea? Open an issue or contact us at [declan@transparency-x.com](mailto:declan@transparency-x.com).
