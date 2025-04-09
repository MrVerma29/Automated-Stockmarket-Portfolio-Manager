# 📊 Automated Stock Market Portfolio Manager

This project is a complete solution for managing and tracking stock market investments using **Excel**, **Google Sheets**, **Power BI**, and **live stock price APIs**. Designed for stockbrokers or portfolio managers, it enables automated tracking of share purchases and sales, real-time performance monitoring, and visual reporting across multiple clients.

---

## 🚀 Project Overview

The system helps efficiently manage multiple client portfolios, monitor individual share performance, and automate key investment insights with minimal manual effort.

It integrates:
- **Google Sheets / Excel** – for structured data entry and automation
- **Stock Broker APIs** – for live share prices (e.g., Motilal Oswal)
- **Power BI** – for advanced dashboards and performance tracking

---

## 🧱 Key Components

### 📒 Excel / Google Sheets Workbook

The workbook contains multiple sheets to manage data for **Clients**, **Shares**, **Holdings**, and **Portfolio Summaries**. Conditional formatting and formulas are used to highlight profit/loss and track share performance.

---

### 📂 Sheets & Their Roles

#### 1. **Clients**
- Tracks client info:  
  `Client_Code`, `Client_Name`, `Avg_Traded_Amount`, `Avg_Trade_Frequency`

#### 2. **Shares**
- Monitors each share's key metrics:  
  `Share_ID`, `Share_Name`, `CMP`, `Target_Price`, `Stop_Loss_Price`, `Date_of_Recommendation`

#### 3. **Holdings**
- Tracks all active investments:  
  `Holding_ID`, `Client_Code`, `Share_ID`, `Quantity`, `Avg_Buy_Price`, `Amount_Invested`, `Profit/Loss`, `Date_of_Investment`, etc.  
- **Color-coded:**  
  - 🟥 Red = Loss  
  - 🟩 Green = Profit

#### 4. **Sold Shares**
- Shows shares fully sold by clients:  
  `Transaction_ID`, `Sold_Quantity`, `Selling_Price`, `Sold_Date`, `Profit/Loss`, etc.

#### 5. **Portfolio**
- Active client portfolios:  
  `Client_Code`, `Current_Portfolio_Value`, `Portfolio_PL%`, `Total_Invested_Amount`, etc.  
- Color-coded for quick insights.

#### 6. **Closed Portfolios**
- For clients who have sold all holdings:  
  `Client_Code`, `Total_Shares_Sold`, `Total_Profit/Loss`, `Date_Closed`

> 🟨 Yellow-highlighted cells: User input required or automated data via API/server.

---

## 📊 Power BI Dashboards

The workbook is integrated with **Power BI** to create rich, interactive dashboards:

### 1. **Client Holding Overview**
- Visualizes individual holdings with real-time CMP, P/L%, amount invested, and risk indicators.

### 2. **Portfolio Summary**
- Offers a high-level portfolio view per client:  
  total investment, returns, trade frequency, and realized P/L.

### 3. **Share Details**
- Tracks performance of each share across clients with CMP vs. target/stop-loss, filterable by client or stock.

### Power BI Features:
- **Multiple Filters & Slicers** (by client, date, share, P/L%)
- **DAX Calculations** for dynamic KPIs and ratios
- **Icons & Colors** indicate:  
  - 🟢 Safe share  
  - 🔴 At-risk share  
  - 🟡 Hold

---

## 🔌 API Integration

Real-time stock data is fetched using broker APIs (e.g., **Motilal Oswal API**) and dynamically reflected in Excel/Sheets.

### Example Use:
- Automatically update CMP
- Trigger buy/sell suggestions
- Highlight shares at target/stop-loss thresholds

---

## 🛠 Getting Started

### ✅ Prerequisites:
- Microsoft Excel / Google Sheets
- Power BI Desktop
- Broker API access (e.g., Motilal Oswal)

### ⚙️ Setup Steps:

#### Excel / Google Sheets:
1. Open the main workbook and review sheets.
2. Connect API to update **CMP** fields.
3. Customize formulas as needed (`AVERAGEIF`, `COUNTIFS`, `IF`, `TODAY`, etc.)

#### Power BI:
1. Load data from the workbook.
2. Explore dashboards:
   - Holding Overview
   - Portfolio Summary
   - Share Details
3. Use filters to interact and gain insights.

---

## 📈 Key Insights You Get
- Real-time client portfolio health
- Share-wise gain/loss and risk alerts
- Auto-calculated investment metrics (P/L%, days held, avg buy price)
- Filter by client/share for tailored insights

---

## 🧩 Future Enhancements
- 🔄 Integration with more stock broker APIs
- 📈 Predictive analytics for share forecasting
- 📤 Automated daily summary emails for clients
- 📱 Mobile dashboard views (via Power BI Service)

---

## 💬 Final Notes

This project blends **automation**, **live data**, and **rich visualization** to empower stockbrokers and investors with actionable insights and efficient portfolio management tools.
