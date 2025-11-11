---
title: Professional Social Media Analytics Dashboard
emoji: 📊
colorFrom: blue
colorTo: purple
sdk: streamlit
sdk_version: "1.32.0"
app_file: professional_dashboard.py
pinned: false
---

# Professional Social Media Analytics Dashboard

A comprehensive, enterprise-grade social media analytics platform with AI-powered insights, predictive analytics, and professional PDF report generation.

## 🚀 Features

### Core Analytics
- **Real-time Dashboard** - KPIs, engagement metrics, follower growth
- **Multi-Format CSV Support** - Auto-detects Instagram, Facebook, and standard formats
- **Content Performance** - Analyze posts by media type, engagement, and reach
- **Audience Insights** - Demographics, growth forecasts, and retention analysis
- **Time Trends** - Temporal patterns and optimal posting times
- **Predictive Analytics** - ML-powered follower growth and engagement predictions

### Professional Reporting
- **Comprehensive PDF Reports** - Includes all charts, KPIs, and predictive analytics
- **Excel Export** - Multi-sheet workbooks with summary statistics
- **CSV Export** - Raw data export
- **JSON Export** - API-ready structured data

### AI-Powered Features
- Smart recommendations for content optimization
- Predictive follower growth forecasting (7, 14, 30 days)
- Automated insights generation
- Best posting time analysis

## 📋 Requirements

- Python 3.10+
- All dependencies listed in `requirements.txt`

## 🔧 Installation

1. **Clone or download the project**

2. **Install dependencies**
```bash
pip install -r requirements.txt
```

3. **Verify required directories exist**
```bash
mkdir -p data uploads assets
```

4. **Add your logo (optional)**
   - Place `logo small black.png` in the `assets/` folder

## ▶️ Running the Dashboard

### Quick Start
```bash
streamlit run professional_dashboard.py --server.port 8510
```

### Access the Dashboard
Open your browser and navigate to:
```
http://localhost:8510
```

## 📊 Using the Dashboard

### 1. Upload Data
- Navigate to **📤 Upload Data**
- Upload CSV files (supports multiple formats):
  - Instagram Post Exports
  - Facebook Video Analytics
  - Standard format with required columns
- System automatically detects and converts formats

### 2. Explore Analytics
- **🏠 Dashboard** - Overview with KPIs and insights
- **📊 Advanced Analytics** - ML-powered analysis
- **🎬 Content Performance** - Post-level analytics
- **👥 Audience Insights** - Demographics and forecasts
- **⏰ Time Trends** - Temporal analysis
- **🔮 Predictive Analytics** - Growth predictions

### 3. Generate Reports
- Navigate to **📋 Reports**
- Click **"📊 Generate Comprehensive PDF"**
- Download professional PDF report with all analytics
- Also available: Excel, CSV, and JSON exports

## 📄 Supported CSV Formats

### Instagram Post Export
Columns: `Post ID`, `Account username`, `Permalink`, `Publish time`, `Description`, `Views`, `Reach`, `Likes`, `Comments`, `Shares`, `Saves`, `Post type`

### Facebook Video Analytics
Columns: Date, `3-second video views`, `Reactions`, `Comments`, `Shares`, demographic columns (M, 18-24), etc.

### Standard Format
Required columns: `post_id`, `timestamp`, `caption`, `likes`, `comments`, `shares`, `saves`, `impressions`, `reach`, `follower_count`, `media_type`

## 🎨 Features Overview

### Dashboard Capabilities
✅ Real-time KPI tracking with period-over-period comparison  
✅ AI-generated insights and recommendations  
✅ Follower growth visualization and forecasting  
✅ Top performing posts identification  
✅ Engagement trends analysis  
✅ Media type performance comparison  
✅ Hashtag performance tracking  
✅ Alert system for anomaly detection  

### PDF Report Contents
✅ Executive Summary with all KPIs  
✅ Content Performance Analysis by media type  
✅ Top 10 Performing Posts  
✅ Predictive Analytics (follower growth forecasts)  
✅ AI-Powered Recommendations  
✅ Weekly Engagement Trends  
✅ Professional branding and formatting  

## 🔒 Data Privacy

- All data processing happens locally on your machine
- No data is sent to external servers
- CSV files are processed temporarily and can be deleted after use

## 🛠️ Troubleshooting

### Port Already in Use
```bash
# Kill existing Streamlit processes
taskkill /F /IM streamlit.exe
# Then restart
streamlit run professional_dashboard.py --server.port 8510
```

### Missing Dependencies
```bash
pip install -r requirements.txt --upgrade
```

### PDF Generation Error
```bash
pip install reportlab pillow
```

## 📦 Project Structure

```
social media analysis/
├── professional_dashboard.py    # Main dashboard application
├── data_adapter.py              # CSV format auto-detection
├── dashboard_sections.py        # Dashboard components
├── advanced_techniques.py       # ML analytics
├── requirements.txt             # Python dependencies
├── README.md                    # This file
├── data/                        # Data directory
├── uploads/                     # Upload directory
└── assets/                      # Logo and assets
    └── logo small black.png
```

## 🎯 Best Practices

1. **Data Quality**: Ensure CSV files have consistent date formats
2. **File Size**: For large datasets (>10k rows), processing may take a few seconds
3. **Regular Updates**: Upload new data weekly for accurate trend analysis
4. **Report Generation**: Generate PDF reports after uploading fresh data

## 🚀 Deployment Options

### Local Development
Already configured! Just run:
```bash
streamlit run professional_dashboard.py --server.port 8510
```

### Network Access
To access from other devices on your network:
```bash
streamlit run professional_dashboard.py --server.port 8510 --server.address 0.0.0.0
```

### Cloud Deployment (Streamlit Cloud)
1. Push code to GitHub
2. Connect to Streamlit Cloud
3. Deploy with one click

## 📞 Support

For issues or questions:
- Check the console for error messages
- Verify all dependencies are installed
- Ensure CSV format matches one of the supported formats

## 📈 Version

**Version:** 2.0  
**Last Updated:** 2025  
**Framework:** Streamlit  
**Python:** 3.10+

## ✨ What's New in v2.0

- ✅ Comprehensive PDF report generation with all analytics
- ✅ Predictive analytics using Linear Regression
- ✅ AI-powered recommendations
- ✅ Multi-format CSV auto-detection
- ✅ Enhanced UI with professional styling
- ✅ NaN-safe data processing
- ✅ Radio button navigation for better UX
- ✅ Excel export with multi-sheet support

---

**© 2025 Professional Social Media Analytics Platform. All Rights Reserved.**
