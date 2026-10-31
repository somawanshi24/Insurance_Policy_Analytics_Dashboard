# Business Requirements Document (BRD)

**Project:** Insurance Policy Analytics Dashboard | Power BI

This BRD was written for the business scenario described in the README. The company and stakeholder roles are fictional; the data is an ExcelR training dataset. For the detailed functional specification, see the [FRD](FRD.md).

## 1. Document control

| Item | Detail |
|---|---|
| Project | Insurance Policy Analytics Dashboard |
| Project type | ExcelR group project (training dataset) |
| Author | Neha Somawanshi (data model, DAX measures, dashboard design, written insights) |
| Status | Delivered |

## 2. Purpose and scope

**Purpose.** Give insurance management one interactive view of customers, policies, premium growth and retention, so they can see what drives the business and where it is losing customers.

**In scope**
- A Power BI dashboard on 5,000 customers and 5,000 policies
- KPIs on policies, customers, claims, coverage and premiums
- Breakdowns by policy status, age range, gender, policy type and policy end year
- A premium growth rate trend over time
- Written insights and recommendations inside the dashboard

**Out of scope**
- Forecasting or predictive models
- Live data refresh from a source system
- Root-cause analysis of why policies end or why growth fell

## 3. Stakeholders

| Stakeholder | Role | Interest |
|---|---|---|
| Senior management | Requester and decision maker | One view of business health and clear priorities |
| Sales and marketing team | Dashboard user | Which policy types and age groups to target for cross-selling |
| Customer retention team | Dashboard user | How many policies are active and where customers are lost |
| Analytics team (author) | Builder | A clear, maintainable dashboard |

## 4. Business problem and objectives

An insurance company holds 5,000 customers and 5,000 policies and has no single view that answers its main questions.

| ID | Objective | Success measure |
|---|---|---|
| BO-1 | Understand which policy types and customer segments drive the business | Policy counts shown by type, age range and gender |
| BO-2 | Track how average premium growth has changed over time | Growth rate trend shown by year |
| BO-3 | Show how many policies are active and where customers are lost | Active Policy % and policy status breakdown |
| BO-4 | Tell management what to prioritise next | Written insights and recommendations |

## 5. Business requirements

| ID | Requirement | Objective | Priority |
|---|---|---|---|
| BR-1 | Show headline KPIs: total policies, total customers, total claim amount, average coverage amount, average premium amount and active policy % | BO-1, BO-3 | Must |
| BR-2 | Break policies down by policy type, age range and gender | BO-1 | Must |
| BR-3 | Show policy status (active or not) and the distribution of policy end years | BO-3 | Must |
| BR-4 | Show the average premium growth rate over time | BO-2 | Must |
| BR-5 | Present written findings and a recommendation that quantify each point | BO-4 | Must |
| BR-6 | Let users move easily between views | All | Should |
| BR-7 | Keep the design consistent and easy to read for non-technical users | All | Should |

## 6. Assumptions and constraints

- The data is a training dataset, so findings do not apply directly to a real insurer.
- The dataset holds one policy per customer on average (5,000 customers, 5,000 policies).
- The dashboard shows how many policies are inactive, but the data does not explain why they ended.
- The dashboard is built in Power BI Desktop and shared as a `.pbix` file.

## 7. Risks

| Risk | Impact | Response |
|---|---|---|
| Only 33.64% of policies are active | Retention is a major business concern | Highlighted as the top finding; renewal campaigns recommended |
| Average premium growth fell to -6.63% in 2023 and -3.98% in 2024 | Revenue growth under pressure | Shown in the growth trend; investigating causes recommended |
| Policy mix is fairly even across types | No single product to rely on | Recommend cross-selling to Health policyholders and the strongest age segments |
| Findings rest on a training dataset | Limited real-world value | Stated as a constraint |

## 8. Acceptance criteria

- The dashboard shows all six KPIs and they match the source data.
- Policy type, age range, gender, policy status and end year breakdowns are available.
- The premium growth trend is shown by year.
- Each written insight includes a figure from the data and ends with a recommendation.
- Users can move between the Overview, Key Insights and Growth Rate views using on-screen buttons.

---

Back to the [project README](README.md).
