# Task 05 — E-commerce Return Rate Investigation

## Problem Statement
Investigate high product return rates in an e-commerce platform using statistical 
analysis and EDA to identify root causes and recommend business actions.

## Dataset Description
- 10,999 orders with 25 features
- Columns: Order details, Product Category, Shipment Mode, Delivery Days, 
  Customer Rating, Discount, Risk Score, Return Flag, Customer Segment

## Statistical Methods Used
- Descriptive Statistics (Mean, Median, Std, Quartiles)
- Correlation Heatmap
- IQR & Z-Score Outlier Detection
- Independent T-Test (Hypothesis Testing)
- Cross-tabulation for Category Return Rates

## Return Findings
- Overall return rate: **70.38%**
- Furniture (71.64%) and Sports (71.26%) have highest return rates
- Returned orders have significantly higher Delivery Days (T-stat: 54.41, p < 0.05)
- Hypothesis: Delivery delay significantly impacts return behavior ✅ Confirmed

## Visual Insights
- Category return rates are nearly uniform (~69–72%) across all categories
- Returned orders show much longer delivery days (median ~9–10 days vs ~5 days)
- Lower customer ratings strongly associated with returns

## Customer Segments
| Segment | Orders | Revenue Loss |
|---|---|---|
| Loyal Customer | 5323 | ₹77,499 |
| Delayed-Delivery | 2309 | ₹73,331 |
| High-Return Customer | 2236 | ₹72,630 |
| Discount-Driven | 1131 | ₹22,359 |

## Recommendations
1. Reduce delivery time — strongest predictor of returns
2. Improve Furniture & Sports quality/description accuracy
3. Target Delayed-Delivery and High-Return segments with proactive communication
4. Review discount strategy — high discounts may attract low-intent buyers

## Future Scope
- Build a return prediction model (Logistic Regression / Random Forest)
- Real-time return risk scoring at checkout
- A/B test faster shipping vs return reduction

## Tools Used
Python, Pandas, NumPy, Seaborn, Matplotlib, SciPy, Scikit-learn
