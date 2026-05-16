# Optimizing Retail Cross-Selling through Market Basket Association & Affinity Analysis

##  Project Overview
This project shifts a retail store's merchandising from "intuition-based" guesswork to a data-driven strategy. By applying **Association Rule Mining (ARM)** to transactional data, the project uncovers hidden product relationships. These insights provide an actionable blueprint for store layout optimization, targeted product bundling, and inventory scaling. The ultimate goal is to increase **Average Order Value (AOV)** by an estimated **10–15%**.

---

##  Business Problem
* **The Challenge:** High-traffic staples (e.g., Milk, Bread) sell consistently, but **Units Per Transaction (UPT)** and **Average Order Value (AOV)** remain stagnant.
* **The Gap:** Management lacks visibility into product "stickiness" and natural purchasing affinities.
* **The Cost:** Generic marketing campaigns fail to convert, and sub-optimal product placement misses high-margin impulse sales.

---

##  Project Objectives
1. **Discover Hidden Affinities:** Extract actionable purchase patterns using key data mining metrics (Support, Confidence, and Lift).
2. **Optimize Store Layout:** Redesign shelf geometry to maximize aisle-walking exposure and minimize shopper fatigue.
3. **Drive Revenue:** Transition from generic discounts to predictive bundling strategies that lift overall sales transaction value.

---

##  Data Architecture & Tech Stack
* Excel, MySQL, Tableau

### 1. Data Engineering (MySQL)
* Cleaned raw transaction logs and removed anomalies.
* Executed **Long-to-Wide** pivot transformations to structure data for transactional basket analysis.

### 2. Analytics Engine (Tableau Desktop)
* Built **Self-Join logic** directly within Tableau to pair products within the same transaction IDs.
* Created calculated fields to compute core data mining metrics:
  * **Support:** Frequency of the product combination across all transactions.
  * **Confidence:** Probability that product B is purchased when product A is bought.
  * **Lift:** Strength of the association rule over random chance.

### 3. Visualization Layer
* **Co-occurrence Heat Map:** Visualizes product clustering and operational "Hot Zones".
* **Top-N Recommendation Slicer:** An interactive dashboard tool for real-time category management decision support.

---

## Preview
[Dashboard Sreenshot] (https://github.com/akandug/market-basket-affinity-analysis/blob/main/MarketBasket%20Dashboard.PNG )
[Dashboard Sreenshot2] ( )
[Product Rank Engine Sreenshot] ( )


---
##  Strategic Insights

###  Insight 1: "The Trinity" (High Support)
* **Finding:** A massive hot zone exists between **Bread, Butter, and Milk** with over 145 order co-occurrences.
* **Action:** These items are cross-category anchors that draw shoppers through predictable paths.

###  Insight 2: "The Social Mission" (High Confidence)
* **Finding:** **Wine** is the store's Rank 1 "Basket Driver." It frequently pulls high-margin items like Pasta and Tomato Sauce into the transaction.
* **Action:** Wine purchasers show a high willingness to buy completing meal components.

###  Insight 3: "Targeted Rewards" (High Lift)
* **Finding:** A statistically significant Lift value confirms a tight affinity between **Beer, Chips, and Diapers**.
* **Action:** Validates a specific "convenience-driven" shopper persona (e.g., parents on quick evening runs).

---

##  Data-Driven Recommendations

* **"Dinner Night" End-Cap:** Deploy a dedicated end-cap display featuring Wine, Pasta, and Tomato Sauce together to capture immediate impulse cross-sales.
* **Store Geometry Shift:** Relocate high-association staples (Milk and Coffee) to the rear of the store. This forces customers to walk the aisles, increasing exposure to impulse items.
* **Predictive Bundling:** Replace blanket discounts with "Next Best Offer" receipt coupons triggered by real-time basket contents.

---

##  Projected Business Implications


| Focus Area | Operational Impact | Expected Outcome |
| :--- | :--- | :--- |
| **Layout Efficiency** | Shifting store geometry based on the Heat Map reduces customer fatigue while maximizing exposure to high-margin impulse items. |  Optimized Foot Traffic |
| **Inventory Scaling** | Understanding "Coupled Demand" ensures that when an anchor product (Coffee) is promoted, inventory for its associates (Sugar/Milk) scales to avoid stockouts. |  Reduced Lost Sales |
| **Marketing ROI** | Replaces margin-eroding storewide sales with hyper-targeted, high-conversion bundle offers. |  10%–15% Lift in AOV |
 
