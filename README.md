# Mobile Game In-App Purchases Dashboard

## Introduction
This is a personal project I made as a student to explore player behavior and monetization patterns in mobile games.  
The dataset is from Kaggle:  
[Mobile Game In-App Purchases Dataset 2025](https://www.kaggle.com/datasets/pratyushpuri/mobile-game-in-app-purchases-dataset-2025)

I wanted to understand:
- Who spends the most money?
- How do players behave (sessions, age, device)?
- What payment methods or game genres generate the most revenue?

It’s also a practice project for me to improve skills in Power BI, Python, and data storytelling.

---

## Tools and Skills
- **Python (Google Colab):** data cleaning
- **Power BI:** dashboard design, KPIs, DAX formulas  
- **Excel:** quick data checks before importing  

---
## Dataset Characteristics
- Total Records: 3,024 user entries
- Features: 13 columns covering user demographics, gaming behavior, and transaction data
- Target Application: Mobile game monetization analysis, user behavior prediction, and revenue optimization
- Data Quality: Contains realistic null values (~2-5%) to simulate real-world data collection scenarios

---
## Data Processing

All preprocessing was done in Google Colab using Python (Pandas) before importing into Power BI for visualization.

Steps:

1. Data Loading

Imported the original CSV file from Google Drive using pandas.read_csv().

Checked dataset shape, column types, and missing values with df.info() and df.isna().sum().

2. Data Cleaning

Converted LastPurchaseDate column to datetime format.

Removed rows with missing InAppPurchaseAmount (non-paying users).

Filled missing values:

PaymentMethod → "Unknown"

Age → median age

Gender, Country, Device, GameGenre → "Unknown"

3. Verification

Rechecked missing values to confirm no nulls remained.

Ensured column types were consistent for Power BI import.

4. Export

Saved the cleaned dataset as clean_mobile_game_data.csv and downloaded it for dashboard creation.
## Dashboard Structure

### 1. Overview
<img width="1312" height="737" alt="over" src="https://github.com/user-attachments/assets/b4d59c61-37dd-418c-be6c-f82144c76609" />

- **Main KPIs**
- Total Revenue: 296K
- Total Users: 2,888
- Paying Users: 2,831
- ARPPU: 104.65
- **Key Insights**
- Whales account for 59% of total revenue.
- Android users generate slightly higher revenue than iOS.
- Male players contribute around 69% of total spending.
- Revenue peaks in April and July, likely due to seasonal events.
- Top 5 game genres: Racing, Battle Royale, Strategy, MOBA, Fighting.

---

### 2. User Behavior
<img width="1308" height="732" alt="usere" src="https://github.com/user-attachments/assets/0997cb7f-8b3f-4dc8-a910-7212bc287941" />

- **Main KPIs**
- Average Session Length: 20.08 minutes
- Average Revenue per Session: 10.19
- Sessions per User: 10.07
- Conversion Rate: 98.03%
- **Key Insights**
- Players aged 25–54 contribute the majority of total spending.
- Teen players (<18) surprisingly account for over 24% of average revenue, likely due to microtransactions.
- 18–24 group has the lowest contribution, possibly due to lower income or preference for free-to-play gameplay.
- Whales dominate revenue across all age groups, but especially strong in 35–54.
- iOS users lead slightly in revenue per session compared to Android.
- Top spending countries remain Afghanistan, Bangladesh, Canada, India and Russia.

---

### 3. Monetization and Devices
<img width="1307" height="732" alt="weq" src="https://github.com/user-attachments/assets/329256f1-0d9b-4343-a2db-1b4ae212603a" />

- **Main KPIs**
- Average Revenue per Device: 98.75K
- Average Payment Amount per Transaction: 102.58
- Top Payment Method: Debit Card
- Average Revenue per Game Genre: 18.52K
- **Key Insights**
- Debit Card leads as the top payment method, followed by PayPal and Gift Card.
- iOS users spend more per transaction (111) than Android users (95), showing higher ARPPU despite fewer transactions.
- Interestingly, Apple Pay transactions are more frequent on Android, while Google Pay dominates on iOS — suggesting possible data inconsistency or cross-platform usage in the dataset.
- Racing, Battle Royale, and Strategy genres maintain the highest average revenue per user (ARPU), especially for iOS players.
- Debit Cards and Paypal remain the most universal methods across both platforms.

---
## Actionable Insights & Recommendations
1️. Revenue & Player Segmentation

Whales contribute 59% of total revenue → focus on retention and exclusive offers for this group.

Male players dominate spending (≈69%) → optimize marketing creatives and offers by gender.

Revenue peaks in April and July, suggesting seasonal in-game events (e.g., holidays or updates) significantly boost sales → plan similar campaigns quarterly.

2️. Player Behavior & Engagement

Players aged 25–54 account for most spending → target these demographics with mid-to-high tier bundles.

Teen players (<18) surprisingly show high microtransaction frequency → consider budget-friendly bundles or gamified reward loops to sustain engagement ethically.

Average session length (~20 mins) and session count (10 per user) imply strong engagement → adding daily challenges or streak bonuses could extend playtime and boost purchases.

3️. Monetization & Payment Optimization

Debit Card, PayPal, and Gift Card are the top payment methods → streamline these checkout options with in-app recommendations.

Cross-platform payment anomalies (e.g., Apple Pay on Android) may indicate SDK misattribution or cross-device login behavior → worth validating in further data quality checks.

iOS users spend more per transaction (ARPPU 111) → prioritize premium content and event passes for iOS segments.

Maintain investment in Racing, Battle Royale, and Strategy genres — consistently highest ARPU.

## Strategic Takeaways

Retention over Acquisition: Keeping high-value players engaged drives more long-term revenue than chasing new users.

Data Validation Needed: Payment anomalies highlight a need for cleaner user-device tracking in future datasets.

Personalization Wins: Tailoring offers by age, platform, and game genre could raise conversion rates by 5–10%.


