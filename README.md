
# 🍬 Nassau Candy - Fixed Operations Dashboard

**Live App:** https://aqdx8zztjbvng8qwgqfjsr.streamlit.app/

**Bug Fixed: 175.9 days → 5.90 days ✅**

![Status](https://img.shields.io/badge/Status-Live-brightgreen)
![Orders](https://img.shields.io/badge/Orders-4%2C007-blue)
![Lead Time](https://img.shields.io/badge/Lead%20Time-5.90%20days-success)

### 📊 KPIs (Verified Live)
- **Avg Lead Time:** 5.90 days (was 175.9 - critical bug fixed)
- **Total Sales:** $55,584
- **Total Profit:** $36,754
- **Margin:** 66.1%
- **Orders:** 4,007 (Jan 2024 - Dec 2025)

### 🔧 What Was Fixed
The original dataset had date parsing errors causing lead time to calculate as 175.9 days. Fixed by:
1. Cleaning `OrderDate` / `ShipDate` parsing
2. Filtering negative lead times
3. Recalculating `(ShipDate - OrderDate)` correctly = **5.90 days avg**

### 📈 Features
- Monthly Orders Trend (interactive)
- Factory Performance breakdown
- Sales / Profit / Margin metrics
- 100% clean CSV included: `Nassau_Clean_FINAL.csv`

### 🚀 How to Run Locally
```bash
pip install -r requirements.txt
streamlit run main.py
