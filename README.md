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
## Dashboard Structure

### 1. Overview
<img width="1312" height="737" alt="over" src="https://github.com/user-attachments/assets/b4d59c61-37dd-418c-be6c-f82144c76609" />

- **Main KPIs**
Total Revenue: 296K
Total Users: 2,888
Paying Users: 2,831
ARPPU: 104.65
- **Key Insights**
Whales account for 59% of total revenue.
Android users generate slightly higher revenue than iOS.
Male players contribute around 69% of total spending.
Revenue peaks in April and July, likely due to seasonal events.
Top 5 game genres: Racing, Battle Royale, Strategy, MOBA, Fighting.

---

### 2. User Behavior
<img width="1308" height="732" alt="usere" src="https://github.com/user-attachments/assets/0997cb7f-8b3f-4dc8-a910-7212bc287941" />

- **Main KPIs**
Average Session Length: 20.08 minutes
Average Revenue per Session: 10.19
Sessions per User: 10.07
Conversion Rate: 98.03%
- **Key Insights**
Players aged 25–54 contribute the majority of total spending.
Teen players (<18) surprisingly account for over 24% of average revenue, likely due to microtransactions.
18–24 group has the lowest contribution, possibly due to lower income or preference for free-to-play gameplay.
Whales dominate revenue across all age groups, but especially strong in 35–54.
iOS users lead slightly in revenue per session compared to Android.
Top spending countries remain Afghanistan, Bangladesh, Canada, India and Russia.

---

### 3. Monetization and Devices
<img width="1310" height="733" alt="money" src="https://github.com/user-attachments/assets/eebb5803-5458-4326-9f78-f8192d26e190" />

- **Main KPIs**
Average Revenue per Device: 98.75K
Average Payment Amount per Transaction: 102.58
Top Payment Method: Debit Card
Average Revenue per Game Genre: 18.52K
- **Key Insights**
Debit Card leads as the top payment method, followed by PayPal and Gift Card.
iOS users spend more per transaction (111) than Android users (95), showing higher ARPPU despite fewer transactions.
Interestingly, Apple Pay transactions are more frequent on Android, while Google Pay dominates on iOS — suggesting possible data inconsistency or cross-platform usage in the dataset.
Racing, Battle Royale, and Strategy genres maintain the highest average revenue per user (ARPU), especially for iOS players.
Debit Cards and Paypal remain the most universal methods across both platforms.

---


