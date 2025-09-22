# Grab Fare & ETA Estimator (C++)

## 📌 Overview
This is a simple interactive program inspired by **Grab** ride-hailing. It estimates:
- **ETA (minutes)**
- **Fare (RM)** including surge multiplier and loyalty discounts

The logic is based on our **Part 1 Innovation Model (Disruptive Innovation)**:
- **Dynamic Surge Pricing** → adapts when demand is higher than supply
- **Grab Pool option** → cheaper access point (low-end disruption)
- **Tier Discounts** → sustaining innovation for loyal users

---

## 🛠️ Features
- Input questions (distance, time, demand, supply, tier, service type)
- Adjusted ETA for peak/off-peak traffic
- Surge multiplier (up to 3.5x)
- Loyalty tier discounts (Basic / Silver / Gold)
- Fare recommendation: suggests Pool during high surge short trips

---

## ▶️ How to Run

### Option 1 – Online Compiler (no typing needed)
1. Paste the code into an online compiler (e.g., Replit, OnlineGDB).
2. Edit the **preset values** at the top of the file:
   ```cpp
   double distance = 6.0;  // km
   int hour = 18;          // 0–23
   int demand = 9;         // 1–10
   int supply = 3;         // 1–10
   int tier = 2;           // 1=Basic, 2=Silver, 3=Gold
   int service = 1;        // 1=Standard, 2=Pool
