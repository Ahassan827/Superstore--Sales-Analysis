# 📊 Sales Profit Margin Analysis — Superstore Dataset



## Business Problem: 

Why is the profit margin flat despite growing sales?



## 📊 Dataset Overview



 -  Number of rows: 9995
           
 -  Number of columns: 24
             
 -  Data Source: Kaggle
         
 - Tool :Excdel
          
 -  Period: 2014 - 2017   

  

## 🧹 Data Cleaning 

✅ Standardized data types (numeric, categorical, date

✅ Checked for blanks and duplicates across all columns

✅ Validated discount values — no outliers above 100% or below 0%

✅ Confirmed date columns parsed correctly for Year / Month / Quarter extraction



## ⚙️ Engineered Columns & Calculated Fields

1- Added Columns - Weighted Discount : (= Discount * Sales)

Why? A simple average treats a $100 order the same as a $10,000 order. Weighting by sales ensures larger orders carry proportional influence.


2- Calculated Fields in PivotTable :

Weighted Avg Discount      = SUM(Weighted Discount) / SUM(Sales)
Weighted Avg Profit Margin = SUM(Profit) / SUM(Sales)

Both fields reflect true business reality — not a flat average across unequal orders.




## 🔍  Insights :


## Insight 1 — Growth is Misleading

Sales grew +20% in 2017 but Profit only grew +14%. This means the business is expanding its top line without a proportional improvement in the bottom line. On the surface the numbers look healthy, but the gap between sales growth and profit growth is a clear signal that something is quietly eroding the margin.


## Insight 2 — Discount is the Root Cause

The weighted avg discount analysis revealed a consistent pattern across all sub-categories. Every sub-category with a weighted avg discount above 20% ended up generating negative profit. Every sub-category with a discount below 15% remained profitable. This is not a coincidence — discount is directly destroying margin. Copiers with 10% discount generated the highest profit while Tables with 24% discount produced the biggest loss.


## Insight 3 — The Problem Started in 2017 Specifically

This is not a long-standing structural issue. Central Region was actually improving in 2016 when discount dropped and profit turned positive. In 2017 the discount spiked suddenly and profit collapsed again. 

Central Region:
2016 → Discount 16% → Profit +$1.2K  ✅
2017 → Discount 26% → Profit -$7.2K  🔴

A sudden spike like this points to a decision that was made, not a gradual trend — which means it can be reversed.


## Insight 4 — Central Region is the Geographic Problem

The same products are being sold across all four regions. East sells them with lower discounts and generates strong profit. Central sells them with the highest discounts and generates the biggest losses.

East    → Discount 18% → Profit +$12.0K  ✅
West    → Discount 21% → Profit  +$8.7K  ✅
South   → Discount 25% → Profit  +$1.5K  ⚠️
Central → Discount 26% → Profit  -$7.2K  🔴

The product is not the problem. The way Central is selling is the problem.


## Insight 5 — East Region is the Benchmark

East has consistently delivered the lowest discount rates and the highest profit over four years. This proves the business model works. The products are capable of generating healthy margins. The gap between East and Central is not a product gap — it is an execution gap.


## Insight 6 — Machines is the Most Dangerous Shift

Machines was a profitable sub-category in 2016. In 2017 the weighted avg discount jumped significantly and it became loss-making within a single year.

Machines:
2016 → Discount 16% → Profit +$2.9K  ✅
2017 → Discount 26% → Profit -$2.8K  🔴

This is the clearest evidence that discount decisions — not market conditions or product quality — are driving the margin problem.


## ✅ Recommendations


🔴 Immediate — Implement a Discount Cap Policy

The data shows a clear threshold where profit turns negative. A maximum discount limit needs to be set for Tables, Machines, and Binders. Any discount above that threshold should require management approval and cannot be granted by a sales rep independently.


🔴 Immediate — Investigate Central Region

The numbers show what is happening but not who is doing it. A direct conversation with the Central sales manager is needed to understand why discounts spiked in 2017 and whether it was driven by customer pressure, sales targets, or individual rep behavior. The answer will determine the right corrective action

.
🟡 Short Term — Tie Sales Incentives to Profit not Revenue

If the sales team is measured only on revenue they will keep offering discounts to close deals regardless of the margin impact. Adding profit margin as a KPI in performance evaluation aligns the team's behavior with the actual business goal.


🟢 Strategic — Replicate the East Model

Before changing products or prices, understand what East is doing differently and apply it to Central and South. The opportunity is already inside the business — it just needs to be scaled.


