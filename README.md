BrightTV Viewership Analytics

Turning subscriber viewing behaviour into actionable insights for subscription growth

**BrightTV Viewership Analytics** is a data analytics case study focused on understanding how subscribers consume BrightTV content and identifying opportunities to increase engagement and grow the subscription base.

The project analyses **9,995 viewing sessions and 4,448 verified subscriber profiles**, examining viewing trends across time, days of the week, channels, provinces, age groups, and gender. The analysis was developed to support the **Customer Value Management (CVM)** team with data-driven recommendations for increasing consumption and acquiring new subscribers.

---

## Table of Contents

* [Background](#-background)
* [Project Overview](#-project-overview)
* [Business Questions](#-business-questions)
* [Data Structure Overview](#-data-structure-overview)
* [Data Preparation & Quality Control](#-data-preparation--quality-control)
* [Key Findings](#-key-findings)
* [Recommendations](#-recommendations)
* [Visual Helper](#-visual-helper)
* [How to Use This Project](#-how-to-use-this-project)
* [User Instructions](#-user-instructions)
* [Contributor Expectations](#-contributor-expectations)
* [Tools & Technologies](#-tools--technologies)
* [Project Limitations](#-project-limitations)
* [Conclusion](#-conclusion)

---

#  Background

BrightTV's CEO set a business objective to **grow the company's subscription base during the financial year**. The CVM team therefore needed insights based on actual subscriber behaviour rather than assumptions.

The case study provided user-profile and viewer-transaction data, with each viewing session represented as an individual record. The analysis was required to investigate user and usage trends, identify factors influencing consumption, recommend content for low-consumption days, and propose initiatives that could grow BrightTV's user base.

An important part of the analysis was ensuring that the dataset was reliable before drawing conclusions. The project therefore included data cleaning, standardisation, duplicate removal, validation, handling of missing values, and conversion of UTC timestamps into South African time (SAST), as required by the case study.

---

#  Project Overview

This project takes a **data-driven approach to understanding BrightTV's viewing behaviour**.

The analysis moves through four main stages:

**1. Data Preparation**
Clean, standardise and validate the subscriber and viewing-session data.

**2. Exploratory Analysis**
Analyse consumption patterns across time, channels, days, provinces, age groups and gender.

**3. Insight Generation**
Identify the factors associated with increases and decreases in viewing activity.

**4. Business Recommendations**
Translate the findings into practical initiatives that CVM could use to improve engagement and support subscriber growth.

The overall objective is not simply to report numbers, but to answer:

> **What does subscriber behaviour tell us about where BrightTV should focus its content, engagement and acquisition efforts?**

---

#  Business Questions

The analysis was designed around four key business questions:

### 1. What are the user and usage trends on BrightTV?

Understand how viewing behaviour changes over time and across different subscriber groups.

### 2. What factors influence consumption?

Investigate the relationship between consumption and factors such as:

* Time of day
* Day of week
* Live sports fixtures
* Geography
* Subscriber demographics
* Channel/content type

### 3. What content could increase consumption on low-consumption days?

Identify patterns in the lowest-consumption days and recommend content or engagement strategies that could improve viewing.

### 4. What initiatives could grow BrightTV's subscriber base?

Identify under-served audience segments and geographic areas where acquisition opportunities may exist.

---

#  Data Structure Overview

The project uses two main categories of information:

### 👤 Subscriber Profile Data

The profile data provides information about BrightTV subscribers, including attributes such as:

| Field               | Description                        |
| ------------------- | ---------------------------------- |
| User ID             | Unique subscriber identifier       |
| Age                 | Subscriber age                     |
| Gender              | Subscriber gender                  |
| Name / Surname      | Subscriber profile information     |
| Race                | Subscriber demographic information |
| Province            | Subscriber location                |
| Social Media Handle | Subscriber profile attribute       |

###  Viewing Session Data

The viewing data records individual subscriber viewing activity.

Each session represents **one record**, meaning that every time a subscriber has a viewing session, a corresponding transaction/session record exists.

Key analytical fields include:

| Field     | Description                            |
| --------- | -------------------------------------- |
| User ID   | Links viewing activity to a subscriber |
| Channel   | Channel/content being viewed           |
| Timestamp | Date and time of viewing               |
| Duration  | Length of the viewing session          |

The two datasets can therefore be combined through the subscriber identifier to analyse **who is watching, what they are watching, and when they are watching**.

---

#  Data Preparation & Quality Control

Before analysing the data, several data-quality checks were performed.

### Cleaning activities included:

* Removing incomplete placeholder profiles
* Removing exact duplicate viewing sessions
* Identifying the correct subscriber ID for joining datasets
* Standardising channel names
* Converting blank values and NULL values into a consistent `Unknown` category
* Identifying age outliers
* Converting timestamps from UTC to South African Standard Time
* Validating the resulting dataset before analysis

### Quality-control results

The analysis identified:

* **918 incomplete profiles** that were removed
* **5 exact duplicate sessions** that were removed
* **5 age outliers** excluded specifically from age-band analysis
* Approximately **700 missing/blank values** across several demographic fields
* An inconsistent secondary user ID column, while the primary `UserID0` field provided a consistent join key

The cleaning process helped ensure that the analysis was based on meaningful subscriber and session records rather than duplicate, placeholder or incorrectly formatted data.

---

#  Key Findings

##  1. Viewing consumption increased over the quarter

Weekly viewing sessions increased from approximately **508 sessions in Week 1 to 1,405 sessions in Week 13**, representing almost a threefold increase.

The strongest acceleration occurred from approximately Week 7 onwards, coinciding with increased live cricket and SuperSport fixture activity.

---

##  2. Live sport is a major consumption driver

SuperSport Live Events and ICC Cricket World Cup content produced some of the strongest viewing spikes in the dataset.

SuperSport Live Events increased substantially from midweek into Thursday–Saturday, while cricket showed a particularly strong Wednesday spike.

This suggests that **live sports fixtures are an important driver of viewing behaviour**.

---

##  3. Viewing varies significantly by day

Monday was the quietest overall viewing day, with approximately **956 sessions**, compared with **1,673 sessions on Friday**.

The analysis therefore identified an opportunity to use targeted programming and engagement strategies to improve consumption on historically weaker days.

---

##  4. Viewership is geographically concentrated

**Gauteng and the Western Cape account for approximately 56.5% of total viewership.**

Meanwhile, Free State, North West and Northern Cape together contribute less than 9%.

This concentration highlights potential acquisition opportunities in lower-consumption provinces.

---

## 👥 5. The audience is strongly concentrated among males aged 25–44

Approximately **90% of sessions come from male subscribers**, while the **25–34 age group accounts for approximately 43% of sessions**.

The 45+ audience represents approximately 12% of sessions, suggesting a potential opportunity to develop content and engagement strategies for older audiences.

Female audiences are also comparatively under-represented in the viewing data.

---

##  6. Time of day affects consumption

Viewing activity increases significantly during key parts of the day.

Sessions increase sharply between approximately **4am and 8am**, while strong consumption is maintained from approximately **10am through 9pm**.

The period around **2am–4am represents very low consumption**, creating a clear distinction between high- and low-activity time periods.

---

# 💡 Recommendations

## 1. Create a Monday Replay Block

Use Monday evening prime time to replay the strongest weekend SuperSport and cricket highlights.

**Why?**

Monday is the lowest-consumption day, while live sport is one of the strongest consumption drivers.

---

## 2. Develop a Sunday Family Viewing Slot

Schedule family-oriented content such as Cartoon Network or Boomerang earlier on Sunday afternoon.

This could help increase Sunday consumption while targeting audiences that may not be strongly represented in the current viewing base.

---

## 3. Use Targeted Push Notifications

Introduce SMS or app notifications on historically low-consumption days.

Notifications should be timed around the identified **5pm–9pm peak window** to encourage subscribers to return to the platform.

---

## 4. Protect and Promote Live Sports Content

SuperSport and cricket generate some of the largest viewing spikes.

BrightTV could therefore:

* Promote major sporting fixtures in acquisition campaigns
* Build subscriber offers around sports access
* Use major fixtures as acquisition opportunities
* Increase visibility of upcoming sporting events

---

## 5. Target Under-Represented Provinces

Free State, North West and Northern Cape represent a relatively small share of current viewing activity.

Potential strategies include:

* Regional acquisition campaigns
* Partnerships with telecommunications providers
* Data or device bundles
* Regional subscription promotions
* More targeted marketing in under-served provinces

---

## 6. Develop Content for Female and 45+ Audiences

The current audience is heavily concentrated among males aged 25–44.

BrightTV could test content targeting:

* Female audiences
* 45+ audiences
* Lifestyle viewers
* Entertainment audiences
* Family audiences

This could diversify the subscriber base instead of relying heavily on the existing core audience.

---

## 7. Investigate Zero-Duration Sessions

Approximately **8.6% of sessions have a duration of zero seconds**.

This should be investigated because it may indicate application, streaming or user-experience friction.

Improving the experience for these sessions could help protect retention before investing heavily in new subscriber acquisition.

---

#  Executive Summary

The analysis suggests that BrightTV's consumption is:

**Growing + Sport-led + Time-sensitive + Geographically concentrated**

The strongest opportunity is to build on what is already working while deliberately addressing under-served audiences and regions.

### The key strategic message:

> **Use live sport and high-performing time periods to drive engagement, while targeting weaker days, under-represented provinces and under-engaged audience segments to support subscriber growth.**

---

#  Visual Helper

The project includes a CEO presentation that provides visual summaries of the analysis, including:

* Weekly consumption trends
* Sessions by day of week
* Channel consumption
* Provincial viewership
* Age distribution
* Gender distribution
* Consumption drivers
* Business recommendations

 **[View the BrightTV CEO Presentation](./BrightTV_CEO_Presentation.pptx)**

 **[View the BrightTV Case Study](./BrightTV_Case_Study.pdf)**

> **Tip:** Add screenshots of your main dashboard/charts to this README so recruiters can understand the project without opening the presentation.

---

#  User Instructions

### To explore the project:

**1. Clone the repository**

```bash
git clone https://github.com/YOUR-USERNAME/BrightTV-Viewership-Analytics.git
```

**2. Open the project**

Navigate to the downloaded repository folder.

**3. Review the data preparation**

Start with the SQL/data-cleaning scripts to understand how the raw data was prepared.

**4. Explore the analysis**

Review the analytical queries used to investigate:

* Viewing trends
* Time patterns
* Channel performance
* Provincial consumption
* Age groups
* Gender
* Low-consumption days

**5. Review the presentation**

Open the CEO presentation to see how the analytical findings were translated into business recommendations.

---

#  Tools & Technologies

The project demonstrates the use of:

* **SQL** — Data cleaning, transformation and analysis
* **Databricks** — Data processing and analytical environment
* **Excel / spreadsheets** — Supporting analysis and validation
* **Data visualisation** — Communicating trends and insights
* **PowerPoint** — Executive-level storytelling and recommendations
* **GitHub** — Project documentation and portfolio presentation

---

#  Contributor Expectations

Contributions are welcome, particularly contributions that improve the analytical depth or presentation of the project.

When contributing:

1. Keep analyses reproducible.
2. Clearly document any new calculations or transformations.
3. Validate data before introducing new insights.
4. Avoid changing the original results without documenting why.
5. Use clear and descriptive SQL/query naming.
6. Explain the business relevance of new findings.
7. Keep visualisations simple, accurate and easy to interpret.
8. Update the README when adding significant functionality.
9. Do not introduce personal or confidential subscriber information.
10. Clearly distinguish between data-supported findings and assumptions.

---

#  Recommendations for Future Analysis

The current analysis provides a strong view of viewing behaviour, but additional data could make the recommendations more powerful.

### Future analysis could include:

**Subscriber conversion analysis**

Determine which viewing behaviours are associated with becoming or remaining a subscriber.

**Churn analysis**

Identify viewing patterns that may indicate a higher risk of cancellation.

**Content performance**

Measure individual programmes rather than only channels to determine which specific content drives engagement.

**Retention analysis**

Track subscriber activity over time to understand whether increased viewing translates into stronger retention.

**Acquisition analysis**

Compare marketing campaigns, acquisition channels and subscriber growth across provinces.

**Customer segmentation**

Create behavioural segments such as:

* Sports-focused viewers
* Entertainment viewers
* Casual viewers
* Heavy viewers
* Low-engagement subscribers

**Predictive analytics**

Future versions could use Python or machine-learning techniques to predict:

* Subscriber churn
* Content preferences
* High-value subscribers
* Likely conversion
* Low-engagement users

---

#  Project Limitations

The findings should be interpreted within the limitations of the available dataset.

The analysis primarily describes **observed viewing behaviour**. It does not prove that a particular content type directly causes subscription growth.

For example, the relationship between live sport and increased viewing suggests that sport is an important consumption driver, but additional information would be needed to establish a causal relationship between sporting content and subscriber acquisition.

Additional data such as subscription dates, cancellations, marketing campaigns, pricing, device type, programme-level data and customer lifetime value would allow deeper analysis.

---

#  Conclusion

This BrightTV case study demonstrates how subscriber-level viewing data can be transformed into actionable business insights.

The analysis identified clear patterns in **when subscribers watch, what content drives consumption, who makes up the current audience and where viewing is concentrated**.

The strongest opportunities identified are to leverage live sports, improve historically weak consumption days, expand into under-represented provinces, develop content for under-engaged audience segments and investigate potential technical friction indicated by zero-duration sessions.

Ultimately, the project demonstrates the role of a data analyst in moving from:

**Raw Data → Data Quality → Analysis → Insights → Business Recommendations**

rather than stopping at reporting numbers.

---

##  Author

**Dineo Masetla**

Aspiring Data Analyst | SQL | Python | Data Analytics | Data Visualisation

This project was developed as a BrightTV Viewership Analytics case study focused on using data to support customer value management and subscription growth.

---

## ⭐ If you found this project useful

Feel free to explore the repository, review the SQL analysis and presentation, and connect with me on GitHub.

**Thank you for exploring the BrightTV Viewership Analytics project!**
