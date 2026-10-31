# Functional Requirements Document (FRD)

**Project:** Insurance Policy Analytics Dashboard | Power BI

This FRD describes how the dashboard meets the requirements in the [BRD](BRD.md). The business context is fictional and the data is an ExcelR training dataset.

## 1. Document control

| Item | Detail |
|---|---|
| Project | Insurance Policy Analytics Dashboard |
| Author | Neha Somawanshi |
| Tool | Power BI Desktop (data loading and cleaning in Power Query / Excel) |
| Deliverable | `Policy_Analytics_Dashboard.pbix` |
| Related document | [BRD](BRD.md) |

## 2. Data requirements

| ID | Requirement |
|---|---|
| DR-1 | Load customer data (5,000 customers) and policy data (5,000 policies) from the Excel dataset |
| DR-2 | Clean the data in Power Query / Excel before modelling |
| DR-3 | The data must support these fields: policy status, age range, gender, policy type, policy end year, premium amount, coverage amount, claim amount and premium growth rate |
| DR-4 | Customers and policies must be related in the data model so customer details such as age range and gender can be analysed against policies |

## 3. Measures

| ID | Measure | Logic | Used on |
|---|---|---|---|
| M-1 | Total Policy | Count of policies | Overview KPI card |
| M-2 | Total Customer | Count of customers | Overview KPI card |
| M-3 | Total Claim Amount | Sum of claim amounts | Overview KPI card |
| M-4 | Avg Coverage Amount | Average of coverage amounts | Overview KPI card |
| M-5 | Avg Premium Amount | Average of premium amounts | Overview KPI card |
| M-6 | Active Policy % | Active policies divided by total policies | Overview KPI card |
| M-7 | Avg Premium Growth Rate | Average premium growth rate, shown by year | Overview and Growth Rate |

## 4. Pages and visuals

### 4.1 Overview

| ID | Visual | Shows | BR |
|---|---|---|---|
| V-1 | KPI cards | M-1 to M-6 | BR-1 |
| V-2 | Chart | Policy status (active vs not) | BR-3 |
| V-3 | Chart | Policies by age range | BR-2 |
| V-4 | Chart | Customers by gender | BR-2 |
| V-5 | Chart | Policies by policy type | BR-2 |
| V-6 | Chart | Distribution of policy end years | BR-3 |
| V-7 | Chart | Premium growth rate over time | BR-4 |

### 4.2 Key Insights

| ID | Element | Shows | BR |
|---|---|---|---|
| V-8 | Text panels | Written findings on customer base, policy mix, premium growth and retention, plus a recommendation | BR-5 |

### 4.3 Growth Rate

| ID | Visual | Shows | BR |
|---|---|---|---|
| V-9 | Line chart | Average premium growth rate by year | BR-4 |

## 5. Navigation and interaction

| ID | Requirement | BR |
|---|---|---|
| F-1 | Buttons at the top of each page to move to Key Insights, Growth Rate and Overview | BR-6 |
| F-2 | Visuals are interactive in Power BI Desktop | BR-6 |
| F-3 | Consistent colors, fonts and layout across all pages | BR-7 |

## 6. Non-functional requirements

| ID | Requirement |
|---|---|
| NFR-1 | The `.pbix` file opens in the free Power BI Desktop |
| NFR-2 | The data model and measures can be refreshed from the Excel dataset |
| NFR-3 | Every written insight quantifies the finding where possible |

## 7. Validation checks

These checks compare the dashboard with the figures reported in the README.

| ID | Check | Expected result |
|---|---|---|
| T-1 | Total Customer and Total Policy | 5,000 each |
| T-2 | Policies by type | Health 1,316, Property 1,236, Life 1,234, Auto 1,214 |
| T-3 | Largest age band | 28 to 37, with 790 policies |
| T-4 | Active Policy % | 33.64% |
| T-5 | Premium growth peak | 4.79% in 2022 |
| T-6 | Premium growth in later years | -6.63% in 2023 and -3.98% in 2024 |
| T-7 | Average growth rate across all years | -1.91% |
| T-8 | Gap between highest and lowest growth rate | 14.53 percentage points |

## 8. Traceability

| Business requirement | Functional requirements |
|---|---|
| BR-1 | M-1 to M-6, V-1 |
| BR-2 | V-3, V-4, V-5 |
| BR-3 | M-6, V-2, V-6 |
| BR-4 | M-7, V-7, V-9 |
| BR-5 | V-8, NFR-3 |
| BR-6 | F-1, F-2 |
| BR-7 | F-3 |

---

Back to the [project README](README.md) or the [BRD](BRD.md).
