## 📦 Data Overview

This project is built on a diverse set of data sources that capture the multi-dimensional impact of the US-China trade war from 2018 to 2023. The data falls into four primary categories:

---

### 1. 🇺🇸🇨🇳 Bilateral Trade Data (US-China)
- **Source:** UN Comtrade Database
- **Files:**  
  - `TradeData_USA_China.csv` — US-reported trade flows with China  
  - `TradeData_China_USA.csv` — China-reported trade flows with the US
- **Years Covered:** 2018–2025
- **Content:** Annual import/export values per product (HS code), reported by each country.
- **Purpose:** Analyze trade volume shifts, identify trade imbalances, and cross-check reporting differences between the US and China.

---

### 2. 📜 Historical Tariff Data
- **Source:** Harmonized Tariff Schedule of the United States (HTSA) + USTR Section 301 tariff notices
- **Files:** `HTS_Tariff_2018_to_2023.csv` (processed from official PDFs)
- **Content Includes:**
  - MFN rates, special duties, and Section 301 additional tariffs
  - Effective dates for policy changes (`begin_effect_date`, `end_effective_date`)
  - Commodity-level detail (HTS-8 codes)
  - Trade agreement indicators (e.g., NAFTA, USMCA, APTA)
- **Purpose:** Establish a timeline of tariff events and link them to specific commodities affected.
# Historical HTSA Files Used for Tariff Analysis (2018–2023)
Year HTSA Revision(s) Description Relevance to US-China Trade War
2018 Rev. 6 / 8 / 14.1 Covers the implementation of Section 301 List 1 and List 2 tariffs Critical year—tariffs began in July 2018

2019 Rev. 1 / 7 / 10 / 15 Includes List 3 and List 4A, as well as the initially scheduled but postponed List 4B tariffs Multiple rounds of tariff escalation and policy updates

2020 Rev. 1 / 10 Reflects exemptions and restorations of certain tariffs Significant changes due to Section 301 exclusions

2021 Rev. 3 / 10 Minor adjustments and continued maintenance of existing exclusions Reflects stabilization of tariff policy

2022 Rev. 3 / 10 No major new tariff policies, but includes transitional entries Useful for checking policy continuation or small adjustments

2023 Rev. 5 / 10 Documents updates related to reinstatement of expired exclusions Latest status for concluding comparative analysis

---

### 3. 🌐 Other Countries' Trade Impact
- **Source:** UN Comtrade, WITS, OECD
- **Files:** e.g., `Trade_OtherCountries_Exports.csv`, `Trade_OtherCountries_Imports.csv`
- **Content:** Global trade flows between third-party countries and both the US and China.
- **Purpose:** Understand trade diversion and substitution effects—e.g., whether ASEAN, EU, or Latin American nations benefited from shifting supply chains.

---

### 4. 📈 Trade Volume & Macroeconomic Indicators
- **Sources:** UN Comtrade (volume), World Bank, FRED, OECD (macroeconomics)
- **Planned Files:**
  - `TradeVolume_Detailed.csv` — includes trade quantities (tons, units) by product and year
  - `MacroIndicators.csv` — includes GDP, inflation, unemployment data by country
- **Purpose:** Provide a broader economic context and support correlation analysis between tariffs, trade activity, and economic trends.

---

All datasets have not been preprocessed and cleaned.

