# Insurance Policy Analytics Dashboard | Power BI

An interactive Power BI dashboard that turns raw insurance policy data into clear, actionable insights on customers, policies, premium growth and retention.

> **Project type:** ExcelR group project (training dataset). I built the data model, DAX measures, dashboard design and written insights in Power BI.

---

## 📸 Dashboard Preview

| Overview | Key Insights |
|----------|--------------|
| ![Overview](images/overview.png) | ![Key Insights](images/key-insights.png) |

*(Add your two screenshots to an `images/` folder with these names.)*

---

## 🎯 Business Problem

An insurance company holds **5,000 customers and 5,000 policies**. Management needs a single view that answers:

1. Which policy types and customer segments drive the business?
2. How has the average premium growth rate changed over time?
3. How many policies are still active, and where is the company losing customers?
4. What should the business prioritise next?

---

## 📊 Dashboard Pages

| Page | What it shows |
|------|---------------|
| **Overview** | KPI cards, policy status, age range, gender, policy type, end-year distribution, premium growth rate |
| **Key Insights** | Written findings and recommendations |
| **Growth Rate** | Average premium growth rate trend |

**KPIs tracked:** Total Policy, Total Customer, Total Claim Amount, Avg Coverage Amount, Avg Premium Amount, Active Policy %

---

## 🔍 Key Insights

1. **Customer and policy base:** 5,000 customers hold 5,000 policies, about one policy per customer. This points to a cross-selling opportunity. Customers are fairly balanced across genders (about 32% to 34% each).
2. **Policy mix:** Health has the most policies (1,316), followed by Property (1,236), Life (1,234) and Auto (1,214). The split is fairly even. The largest age band is 28 to 37 (790 policies), and 38 to 47 (737) and 58 to 67 (764) follow closely.
3. **Premium growth trend:** Average premium growth peaked at **4.79% in 2022**, then fell to **-6.63% in 2023** and **-3.98% in 2024**. The gap between the highest and lowest growth rates is **14.53 percentage points**, and the average growth rate across all years is **-1.91%**.
4. **Retention is the biggest concern:** Only **33.64%** of policies are active. The active to inactive ratio is **0.51 : 1**, so roughly two out of three policies are terminated or lapsed.
5. **Recommendation:** Prioritise renewal and retention campaigns, investigate the causes behind the recent growth decline, and cross-sell to the strongest age segments and to Health policyholders.

---

## 🛠️ Tools and Skills

- **Power BI Desktop:** data modelling, interactive visuals, page navigation buttons
- **DAX:** KPI measures (totals, averages, active policy %, growth rate)
- **Power Query / Excel:** data loading and cleaning
- **Visuals used:** KPI cards, pie and donut charts, bar charts, line chart, text and shape elements

---

## 📁 Repository Structure

```
├── README.md
├── Policy_Analytics_Dashboard.pbix
├── Dataset/
│   └── policy_data.xlsx
└── images/
    ├── overview.png
    └── key-insights.png
```

*(Update file names to match your repo.)*

---

## ▶️ How to Open

1. Download `Policy_Analytics_Dashboard.pbix`.
2. Open it in **Power BI Desktop** (free from Microsoft).
3. Use the **Key Insights**, **Growth Rate** and **Overview** buttons at the top to move between views.

---

## 💡 What I Learned

- Turning raw data into a story that ends with a clear recommendation, not just charts
- Building KPI measures in DAX and designing a consistent, readable dashboard
- Writing insights that quantify the finding (growth gap, retention ratio) and suggest a next step

---

## 👩‍💻 Author

**Neha Somawanshi**
[LinkedIn](https://www.linkedin.com/in/nehasomawanshi791378308) | [GitHub](https://github.com/somawanshi24) | nehausomawanshi@gmail.com
