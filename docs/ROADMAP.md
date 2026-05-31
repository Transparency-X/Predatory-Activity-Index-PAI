# Predatory Activity Index for Ireland: Roadmap

---

## 🗺️ **Project Roadmap**

This roadmap outlines the **development, deployment, and scaling** of the **Predatory Activity Index (PAI) for Ireland**. It is divided into **four phases**, each with specific goals, deliverables, and timelines.

---

## 📅 **Phase 1: Prototype (Q2 2026)**

**Goal**: Validate the concept and methodology using mock data.

### **Objectives**

- Define the **index methodology** and **category weights**. 
- Generate **mock datasets** to simulate real-world predatory activity.
- Build the **composite index calculation logic**.
- Create a **prototype visualization** of the PAI.
- Gather **feedback from stakeholders** (e.g., CCPC, Gardaí).

### **Deliverables**


| **Task**                       | **Owner**               | **Timeline** | **Status** | **Output**                                                              |
| ------------------------------ | ----------------------- | ------------ | ---------- | ----------------------------------------------------------------------- |
| Define index methodology       | Transparency-X Team     | April 2026   | ✅ Complete | Methodology document (`docs/methodology.md`)                            |
| Generate mock datasets         | Data Team               | April 2026   | ✅ Complete | Mock data in `data/mock/`                                               |
| Build composite index logic    | Data Team               | May 2026     | ✅ Complete | `src/processing/composite_index.py`                                     |
| Create prototype visualization | Data Team               | May 2026     | ✅ Complete | `outputs/visualizations/ireland_predatory_activity_index_prototype.png` |
| Validate with stakeholders     | Declan (Transparency-X) | June 2026    | ⏳ Pending  | Stakeholder feedback report                                             |


### **Key Milestones**

- **April 2026**: Methodology and mock data finalized.
- **May 2026**: Prototype visualization and composite index logic completed.
- **June 2026**: Stakeholder feedback incorporated; prototype validated.

---

## 🚀 **Phase 2: Minimum Viable Product (MVP) (Q3–Q4 2026)**

**Goal**: Develop a **functional MVP** with real data and basic features.

### **Objectives**

- Integrate **real data** from public sources (e.g., CCPC, Gardaí).
- Develop an **ETL pipeline** for automated data collection.
- Launch a **static dashboard** (updated monthly).
- Secure **pilot partnerships** with 1–2 banks or NGOs.
- Add **geospatial analysis** and **email alerts**.

### **Deliverables**


| **Task**                        | **Owner**               | **Timeline**   | **Status** | **Output**                                        |
| ------------------------------- | ----------------------- | -------------- | ---------- | ------------------------------------------------- |
| Integrate CCPC scam alerts      | Data Team               | July 2026      | ⏳ Pending  | `src/data_collection/scrape_ccpc.py`              |
| Integrate Garda cybercrime data | Data Team               | July 2026      | ⏳ Pending  | `src/data_collection/fetch_garda_data.py`         |
| Develop ETL pipeline            | Tech Team               | August 2026    | ⏳ Pending  | Airflow/Dagster workflows in `.github/workflows/` |
| Launch static dashboard         | Frontend Team           | September 2026 | ⏳ Pending  | Plotly Dash/Streamlit app                         |
| Secure pilot partnerships       | Declan (Transparency-X) | September 2026 | ⏳ Pending  | MOUs with pilot partners                          |
| Add geospatial mapping          | Data Team               | October 2026   | ⏳ Pending  | Folium/Plotly maps in `outputs/visualizations/`   |
| Implement email alerts          | Tech Team               | October 2026   | ⏳ Pending  | SMTP/Twilio integration in `src/alerts/`          |


### **Key Milestones**

- **July 2026**: Real data integration (CCPC, Gardaí).
- **August 2026**: ETL pipeline operational.
- **September 2026**: Static dashboard launched; pilot partnerships secured.
- **October 2026**: Geospatial mapping and email alerts added.

---

## 🌍 **Phase 3: Live Index (2027)**

**Goal**: Deploy a **real-time, production-ready PAI** with advanced features.

### **Objectives**

- Transition to **daily updates** for the dashboard.
- Add **predictive modeling** (e.g., trend forecasting).
- Launch **API access** for third-party integrations.
- Develop a **public reporting portal** for citizen contributions.
- Expand to **EU/UK markets** (e.g., "European Predatory Activity Index").

### **Deliverables**


| **Task**                        | **Owner**         | **Timeline** | **Status** | **Output**                                   |
| ------------------------------- | ----------------- | ------------ | ---------- | -------------------------------------------- |
| Deploy real-time dashboard      | Frontend Team     | Q1 2027      | ⏳ Pending  | Live Plotly Dash/Streamlit app               |
| Add predictive modeling         | Data Science Team | Q1 2027      | ⏳ Pending  | Prophet/ARIMA models in `src/models/`        |
| Launch API access               | Tech Team         | Q2 2027      | ⏳ Pending  | FastAPI/Flask API in `src/api/`              |
| Develop public reporting portal | Frontend Team     | Q2 2027      | ⏳ Pending  | Flask/Django app in `src/portal/`            |
| Expand to EU/UK markets         | Business Team     | Q3 2027      | ⏳ Pending  | Regional indices and partnerships            |
| Add sector-specific indices     | Data Team         | Q4 2027      | ⏳ Pending  | Custom indices for finance, healthcare, etc. |


### **Key Milestones**

- **Q1 2027**: Real-time dashboard and predictive modeling live.
- **Q2 2027**: API access and public reporting portal launched.
- **Q3 2027**: Expansion to EU/UK markets begins.
- **Q4 2027**: Sector-specific indices added.

---

## 📈 **Phase 4: Scaling (2028+)**

**Goal**: Scale the PAI into a **global, self-sustaining platform** with advanced features and monetization.

### **Objectives**

- Introduce **blockchain verification** for data transparency.
- Launch a **mobile app** for on-the-go access.
- Monetize through **subscriptions, API fees, and sponsorships**.
- Partner with **global organizations** (e.g., Transparency International, Europol).
- Develop **AI-driven insights** (e.g., NLP for scam detection).

### **Deliverables**


| **Task**                          | **Owner**               | **Timeline** | **Status** | **Output**                                    |
| --------------------------------- | ----------------------- | ------------ | ---------- | --------------------------------------------- |
| Introduce blockchain verification | Tech Team               | Q1 2028      | ⏳ Pending  | Ethereum/Hyperledger integration              |
| Launch mobile app                 | Mobile Team             | Q2 2028      | ⏳ Pending  | React Native/Flutter app                      |
| Monetize via subscriptions        | Business Team           | Q2 2028      | ⏳ Pending  | Subscription tiers and pricing models         |
| Partner with global organizations | Declan (Transparency-X) | Q3 2028      | ⏳ Pending  | MOUs with Transparency International, Europol |
| Develop AI-driven insights        | Data Science Team       | Q4 2028      | ⏳ Pending  | NLP models for scam detection in `src/ai/`    |
| Add gamification features         | Frontend Team           | 2029         | ⏳ Pending  | Reward system for user engagement             |


### **Key Milestones**

- **Q1 2028**: Blockchain verification and mobile app beta.
- **Q2 2028**: Monetization models launched.
- **Q3 2028**: Global partnerships secured.
- **Q4 2028**: AI-driven insights and gamification added.

---

## 🎯 **Long-Term Vision (2030+)**

### **Global Predatory Activity Index**

- Expand the PAI to **cover 50+ countries**, with **regional and global indices**. 
- Partner with **UN, World Bank, and OECD** to integrate PAI into global policy frameworks.
- Develop **AI-powered early warning systems** for emerging threats (e.g., new scam types, cyberattacks).

### **Sector-Specific Ecosystems**

- Create **dedicated PAI platforms** for:
  - **Finance**: Fraud detection for banks and insurers.
  - **Healthcare**: Exploitation monitoring for hospitals and patients.
  - **Real Estate**: Scam prevention for buyers and renters.
  - **E-Commerce**: Trust scoring for online marketplaces.

### **Decentralized PAI**

- Explore **blockchain-based governance** for the PAI, allowing **community-driven updates** and **transparent data verification**.
- Enable **user-owned data** via decentralized identifiers (DIDs).

---

## 📊 **Success Metrics**


| **Metric**                         | **Phase 1 Target** | **Phase 2 Target** | **Phase 3 Target** | **Phase 4 Target** |
| ---------------------------------- | ------------------ | ------------------ | ------------------ | ------------------ |
| **Data Sources Integrated**        | 5 (mock)           | 10 (real)          | 20+                | 50+                |
| **Dashboard Users**                | 10 (internal)      | 100 (pilot)        | 1,000+             | 10,000+            |
| **API Requests/Month**             | N/A                | 1,000              | 10,000+            | 100,000+           |
| **Public Reports Submitted/Month** | N/A                | 50                 | 500+               | 5,000+             |
| **Revenue (Annual)**               | €0                 | €50K               | €500K+             | €5M+               |
| **Cost Savings for Users**         | N/A                | €1M                | €10M+              | €100M+             |
| **Stakeholder Partnerships**       | 2–3                | 5–10               | 20+                | 50+                |


---

## 🤝 **Collaboration & Partnerships**

### **Current Partners**

- **Transparency-X**: Project lead and development.
- **Mock Data**: Simulated datasets for prototyping.

### **Target Partners (2026–2027)**


| **Organization**           | **Role**                        | **Phase** | **Status** |
| -------------------------- | ------------------------------- | --------- | ---------- |
| CCPC                       | Data provider (scam alerts)     | Phase 2   | ⏳ Pending  |
| Gardaí                     | Data provider (cybercrime)      | Phase 2   | ⏳ Pending  |
| Central Bank of Ireland    | Data provider (fraud)           | Phase 2   | ⏳ Pending  |
| AIB/Bank of Ireland        | Pilot partner (financial data)  | Phase 2   | ⏳ Pending  |
| HSE                        | Data provider (elder abuse)     | Phase 2   | ⏳ Pending  |
| WRC                        | Data provider (workplace cases) | Phase 2   | ⏳ Pending  |
| Transparency International | Global expansion partner        | Phase 4   | ⏳ Pending  |
| Europol                    | EU-wide collaboration           | Phase 4   | ⏳ Pending  |


### **How to Partner**

Interested in collaborating? Contact us at [declan@transparency-x.com](mailto:declan@transparency-x.com) or open a discussion in the [GitHub repository](https://github.com/transparency-x/predatory-activity-index-ireland).

---

## 📅 **Timeline Summary**


| **Phase**  | **Duration** | **Key Focus**                            | **Output**                       |
| ---------- | ------------ | ---------------------------------------- | -------------------------------- |
| Prototype  | Q2 2026      | Methodology, mock data, prototype        | Prototype dashboard              |
| MVP        | Q3–Q4 2026   | Real data, ETL, static dashboard         | MVP with basic features          |
| Live Index | 2027         | Real-time updates, API, reporting portal | Production-ready PAI             |
| Scaling    | 2028+        | Blockchain, mobile app, monetization     | Global, self-sustaining platform |


---

## 💡 **How to Contribute**

1. **Fork the Repository**: Start by forking the [Predatory Activity Index repository](https://github.com/transparency-x/predatory-activity-index-ireland).
2. **Pick an Issue**: Check the [Issues](https://github.com/transparency-x/predatory-activity-index-ireland/issues) tab for open tasks.
3. **Develop**: Work on your feature/fix in a new branch.
4. **Submit a PR**: Open a pull request with your changes.
5. **Join the Discussion**: Share ideas in the [Discussions](https://github.com/transparency-x/predatory-activity-index-ireland/discussions) tab.

---

## 📬 **Feedback & Questions**

Have questions or suggestions for the roadmap?

- Open an issue in the [repository](https://github.com/transparency-x/predatory-activity-index-ireland).
- Contact the team at [declan@transparency-x.com](mailto:declan@transparency-x.com).

---

## 🔗 **Related Documents**

- [README](README.md): Project overview and setup instructions.
- [Overview](OVERVIEW.md): Detailed project vision and impact.
- [Features](FEATURES.md): List of current and planned features.
