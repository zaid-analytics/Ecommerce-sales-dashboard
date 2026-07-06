# 📊 E-commerce Sales Dashboard (Power BI)
Recommended structure and order

## 1. Project Title / Headline
**E-commerce Sales & Profit Analysis Dashboard** — Interactive Power BI report jo sales, profit, quantity aur payment trends ko ek hi jagah visualize karta hai.

## 2. Short Description / Purpose
Ye dashboard ek e-commerce dataset par based hai jo business ke key sales metrics ko track karta hai — jaise monthly profit trend, quantity sold, category-wise performance, state-wise sales aur payment mode distribution. Purpose ye hai ki business owner ya analyst bina raw data khole hi, ek glance mein pata laga sake ki:
- Kaunsa month profitable raha
- Kaunsi category sabse zyada revenue/quantity de rahi hai
- Kaunsa state sales mein aage hai
- Customers zyada kis payment mode ka use kar rahe hain

## 3. Tech Stack
- **Tool:** Microsoft Power BI Desktop
- **Data Modeling:** Star-schema style relationship banayi gayi `Orders` table (Order Date, State, Order Month) aur `Details` table (Category, PaymentMode, Amount, Quantity, Profit) ke beech
- **DAX Measures:** Aggregated measures banaye — `Sum(Profit)`, `Sum(Amount)`, `Sum(Quantity)` — jo cards aur charts mein use hue
- **Calculated Column:** Naya column `Order Month` banaya `Order Date` se, taaki month-wise trend analysis easy ho
- **Visualization Types:** Line Chart, Donut Chart, Pie Chart, Column Chart, KPI Cards, Slicers

## 4. Data Source
Dataset **Kaggle** se liya gaya hai (E-commerce Sales dataset). Do main tables use hui hain:
- `Orders` — Order Date, State
- `Details` — Category, Payment Mode, Amount, Quantity, Profit

## 5. Features & Highlights
- 📈 **Profit by Month** — Line chart jo monthly profit trend dikhata hai
- 📉 **Quantity by Month** — Line chart jo monthly quantity sold track karta hai
- 🍩 **Profit by Category** — Donut chart, category-wise profit contribution
- 💳 **Payment Mode by Amount** — Donut chart, kis payment method se kitna amount aaya
- 🥧 **Quantity by Category** — Pie chart representation
- 📊 **Profit by State** — Column chart, state-wise profit comparison
- 🔢 **KPI Cards** — Total Amount, Total Quantity, Total Profit ek glance mein
- 🎛️ **Interactive Slicers** — State aur Month ke basis par pura dashboard filter kar sakte hain

- Screebsshot / demos
- show what dashboard look like-
- Example: [Dashboard Preview](

---
### 🔗 How to Use
1. `.pbix` file download karke Power BI Desktop mein open karein
2. Slicers (State / Month) use karke data filter karein
3. Visuals par hover/click karke cross-filtering dekhein
