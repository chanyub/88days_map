# 88 Days Map - Working Holiday Visa Areas

Interactive map showing eligible work areas for Australian Working Holiday visa holders to complete their 88-day requirement.

## 🌐 Live Sites

- **Production**: https://chanyub.github.io/88days_map/
- **Staging Demo**: Test `stg` branch locally
  1. Clone the repository: `git clone https://github.com/chanyub/88days_map.git`
  2. Switch to staging: `git checkout stg`
  3. Run local server: `python -m http.server 8000` or `npx serve .`
  4. Open: `http://localhost:8000`

## 🚀 Development Workflow

1. **Development**: Make changes in `stg` branch
2. **Testing**: Run local server to test staging changes
3. **Production**: Create PR from `stg` to `main` → Auto-deploy via GitHub Actions

## ✨ Features

- **Interactive Map**: Australian postcode areas with color-coded work eligibility
- **Search Function**: Find postcodes and localities quickly
- **Information Panels**: Detailed work requirements for each area type
- **Guestbook**: Leave messages with username support
- **Visitor Statistics**: Track site usage with local storage
- **Loading Indicator**: Smooth data loading experience
- **Creator Contact**: Easy email copy and YouTube channel access

## 📊 Work Area Categories

1. **Remote/Very Remote Australia (Red)**: Tourism and hospitality work from 22 June 2021
2. **Australia (Orange)**: Tourism and hospitality work from 22 June 2021 (applications from 1 July 2022)
3. **Northern Australia (Yellow)**: Tourism and hospitality work from 22 June 2021
4. **Regional Australia (Green)**: Specified work (primary industries)
5. **Bushfire Declared Areas (Blue)**: Bushfire recovery work after 31 July 2019
6. **Natural Disaster Areas (Purple)**: Natural disaster recovery work from 31 Dec 2021

## 📂 File Structure

```
├── index.html              # Main application
├── postcode2name.json      # Postcode to locality mapping
├── data/
│   ├── geo_chunk_*.json    # Geospatial data (27 chunks)
│   └── table*.csv          # Work area classifications
└── .github/workflows/
    └── deploy.yml          # Auto-deployment workflow
```

## 🛠 Technologies

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Mapping**: Leaflet.js
- **Data**: GeoJSON, CSV
- **Storage**: LocalStorage for user preferences
- **Deployment**: GitHub Pages via GitHub Actions

## 🚀 SEO & Performance Features

- **Complete SEO Optimization**: Meta tags, structured data, sitemap
- **Google Search Console Ready**: Verification file included
- **PWA Support**: Mobile app-like experience
- **Performance Optimized**: Preloaded resources, efficient loading
- **Analytics Ready**: Google Analytics 4 integration prepared

### Target Keywords
- "working holiday visa 88 days"
- "australian working holiday areas"
- "88 days map australia"
- "working holiday postcode"

## 📧 Contact

Created by **하고싶은게많은🇰🇷**
- Email: somanytube@gmail.com  
- YouTube: [하고싶은게많은](https://www.youtube.com/@%ED%95%98%EA%B3%A0%EC%8B%B6%EC%9D%80%EA%B2%8C%EB%A7%8E%EC%9D%80)

## 📋 Data Sources

Official information from the Australian Department of Home Affairs:
- [Specified Work Requirements](https://immi.homeaffairs.gov.au/what-we-do/whm-program/specified-work-conditions/specified-work-417)

## 🔍 SEO Setup Instructions

1. **Google Search Console**:
   - Add property: https://chanyub.github.io/88days_map/
   - Replace `google-site-verification.html` with Google's verification file
   - Submit sitemap: https://chanyub.github.io/88days_map/sitemap.xml

2. **Google Analytics**:
   - Create GA4 property
   - Replace `G-XXXXXXXXXX` in index.html with your tracking ID
   - Uncomment the gtag config line

3. **Bing Webmaster Tools**:
   - Add and verify your site
   - Submit sitemap

---

> **Note**: This tool is for informational purposes only. Always verify current requirements with official government sources.