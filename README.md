# 📦 Inventory Performance Dashboard

## 📝 Short Description
An interactive Power BI dashboard, backed by SQL analysis, that shows where a retail chain loses sales to stock-outs and where it holds too much unsold stock. It exists to help the business reorder the right products and stop wasting money on overstock.

## 🛠️ Tech Stack
- 🗄️ **MySQL:** data checks, cleaning and KPI queries
- 📊 **Power BI:** dashboard, DAX measures and slicers
  
## 📂 Data Source
Dataset from Kaggle: www.kaggle.com/datasets/atomicd/retail-store-inventory-and-demand-forecasting


## ✨ Highlights

### ❗ Business Problem
A retail chain with many stores, products and regions has stock that does not match customer demand. Some products run short and lose sales, while others are overstocked and tie up money. The business needs to know where this happens, how much it costs, and why.

### 🎯 Goal of the Dashboard
- ✅ Measure how much demand is being met (fill rate) and how often stock-outs happen
- 💸 Find lost units and lost revenue by category, region, store and product
- 📦 Identify overstocked products and slow-moving stock
- 🌦️ Show how promotions, discounts, season, weather and epidemic periods affect demand

### 🖼️ Walkthrough of Key Visuals

**📄 Page 1: Overview**
- 🔢 Cards for total sold, total demand, fill rate %, stock-out rate % and lost revenue
- 📊 Lost revenue by category and by region
- 📈 Monthly demand vs units sold trend
- 🎛️ Slicers for category, region, store and date

**📄 Page 2: Stock-outs & Overstock**
- 🔴 Top 10 products by lost revenue (the "reorder now" list)
- 🟡 Top 10 overstocked products by days of inventory (the "stop ordering or discount" list)
- 🌍 Stock-out rate by region and category
- ⏳ Days of inventory by category
- 🔄 Ordering gap: units ordered vs demand

**📄 Page 3: Demand Drivers**
- 🏷️ Average demand with vs without promotion
- 💲 Average demand by discount
- 🍂 Average demand by season, weather and epidemic period

### 💡 Business Insights
1. 📊 Stores met **85%** of demand. About **1.1M units** (7.9M demand vs 6.8M sold) went unmet, worth **92.8M** in lost revenue.
2. 🚫 Stock-outs happened in **70.3%** of store-product-days, and the rate was similar in every category (67–73%) and region (70–71%), so this is a system-wide issue and not one bad store.
3. 🏆 **Groceries** lost the most revenue (**36M, about 39%** of the total), and the **North** region lost **34M (about 37%)**.
4. 🏷️ Demand was about **30% higher with promotions** (123 vs 95). Discounts of **15–25%** gave similar demand (123–124), and 0–5% discounts gave about 95.

### ✅ Recommendations
1. 🔼 **Raise order quantities by about 15%**, starting with Groceries, the North region and the top lost-revenue products (P0009, P0014, P0011).
2. 📅 **Stock up before promotions and the summer season**, since demand rises sharply in both.
