# BRICS Gold Trade Analysis

This project studies international gold-trade activity involving BRICS countries and selected African reporting countries, with particular attention to changes across the 2017-2023 period. It combines trade records, gold-price reference data, country membership/reference information, validation logic, relational storage, statistical analysis, and Tableau visualization.

## Project objective

The analysis was built to examine how gold imports and exports changed across countries, partners, quantities, values, and time periods, and to compare those observations with supporting information such as gold prices and BRICS membership data.

## Data and analysis flow

1. Collect international gold-trade records from UN Comtrade.
2. Prepare supporting BRICS-country and gold-price reference datasets.
3. Validate required fields and separate records that do not meet the project rules.
4. Standardize units and analysis attributes.
5. Load structured data into relational tables for repeatable querying.
6. Compare trade values, quantities, partners, and time-period patterns.
7. Use statistical analysis to investigate observed relationships.
8. Prepare the final analytical outputs for Tableau dashboards.

## Technologies

- Python and Jupyter Notebook
- Pandas
- UN Comtrade API
- World Bank commodity-price data
- Oracle Database and SQLAlchemy
- SciPy
- SQL
- Tableau
- draw.io

## Project resources

These are the original supporting files linked from the project report.

| Resource | Description | Link |
| --- | --- | --- |
| `Mapping Document.xlsx` | Analysis/mapping workbook containing data used for project assumptions and analysis. | [Open workbook](https://docs.google.com/spreadsheets/d/1P0ebDDR3_nQYbMlxrfiNk52cenHLSGTq/edit?usp=sharing&ouid=114840663789662506255&rtpof=true&sd=true) |
| `Data Validations.xlsx` | Validation workbook containing checked records and rejected-data details. | [Open workbook](https://docs.google.com/spreadsheets/d/1BvPr6GhlXTH28ZcxHXw5sdOzO09X9Ics/edit?usp=sharing&ouid=114840663789662506255&rtpof=true&sd=true) |
| `Brics.xlsx` | BRICS reference data prepared into the format used by the analysis. | [Open workbook](https://docs.google.com/spreadsheets/d/1Hno_HFEBlxc7BYLMc31G0KsxnToYO0EN/edit?usp=sharing&ouid=114840663789662506255&rtpof=true&sd=true) |
| `Gold Price.xlsx` | World Bank gold-price data prepared and converted for use in the research. | [Open workbook](https://docs.google.com/spreadsheets/d/1ggdeVNNf-kWhKJaMk9kJikMMip9_yEoP/edit?usp=sharing&ouid=114840663789662506255&rtpof=true&sd=true) |
| Tableau visualization | Interactive visualizations created from the project outputs. | [Open Tableau dashboard](https://public.tableau.com/views/SignificanceofGoldTradeonBRICSvsOtherCountries/PartnersList?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link) |

## Repository contents

```text
.
├── Source Code.ipynb     # Extraction, cleaning, validation, loading, and analysis
├── Database Tables.sql   # Relational table definitions
├── Gold Trade.drawio     # Data/model diagram
├── media/                # Project figures and report assets
└── README.md
```

## Run the project

Open the notebook and configure the API/database values required by the extraction and loading sections in your local environment.

```bash
jupyter notebook "Source Code.ipynb"
```

## References used in the original analysis

1. [Goldman Sachs — Building Better Global Economic BRICs](https://www.goldmansachs.com/intelligence/archive/building-better.html)
2. [Council on Foreign Relations — How BRICS Got Here](https://www.cfr.org/expert-brief/how-brics-got-here)
3. [Modern Diplomacy — A BRICS reserve currency: exploring the pathways](https://moderndiplomacy.eu/2022/12/21/a-brics-reserve-currency-exploring-the-pathways/)
4. [Chards — BRICS Summit 2023 and a possible gold-backed digital currency](https://www.chards.co.uk/guides/brics-summit-2023-is-the-gold-backed-digital-currency-coming/1198)
5. [Lowy Institute — De-dollarisation and shifting power between the US and BRICS](https://www.lowyinstitute.org/the-interpreter/de-dollarisation-shifting-power-between-us-brics)
6. [Policy Circle — BRICS currency faces challenges](https://www.policycircle.org/opinion/brics-currency-faces-challenges/)
7. [World Bank — Commodity Markets historical monthly data](https://thedocs.worldbank.org/en/doc/5d903e848db1d1b83e0ec8f744e55570-0350012021/related/CMO-Historical-Data-Monthly.xlsx)
8. [BRICS member states reference](https://en.wikipedia.org/wiki/Member_states_of_BRICS)
9. [Forbes — U.S. gold trade analysis](https://www.forbes.com/sites/kenroberts/2021/04/30/with-1-billion-monthly-surplus-us-gold-trade-shaking-off-wild-2020/)
10. [CCN — Gold price discussion](https://www.ccn.com/5-key-reasons-why-golds-price-is-set-to-skyrocket-in-2020/)
11. [ScienceDirect — Is gold a hedge or a safe-haven asset in the COVID-19 crisis?](https://www.sciencedirect.com/science/article/pii/S0264999321001772)
12. [Bloomberg — African gold trade and suspected smuggling](https://www.bloomberg.com/news/features/2021-12-28/where-does-gold-come-from-in-africa-suspected-smuggling-to-dubai-rings-alarms)
13. [Financial Post — Zijin Mining / Continental Gold](https://financialpost.com/commodities/mining/chinas-zijin-mining-agrees-to-buy-canadas-continental-gold-for-about-1-bln)
14. [TradeImeX — Switzerland gold trade statistics](https://tradeimex.in/blogs/switzerland-gold-trade-import-export-statistics-of-2023)
15. [CBC — Canada gold reserves](https://www.cbc.ca/news/business/gold-canada-reserves-1.3475818)
16. [Forbes Advisor — USD/CAD forecast](https://www.forbes.com/advisor/money-transfer/usd-cad-forecast/)
17. [Corruption Watch — Gold laundering](https://www.corruptionwatch.org.za/delving-into-the-shady-world-of-gold-laundering/)
18. [Daily News Egypt — Egypt gold exports](https://www.dailynewsegypt.com/2023/07/16/egypts-gold-exports-decline-by-45-in-5m-2023/)
19. [The Star — Kenya and South Africa trade barriers](https://www.the-star.co.ke/news/2023-01-11-where-kenya-south-africa-should-start-to-address-trade-barriers/)
20. [Kitco — Gold-price trajectory discussion](https://www.kitco.com/opinion/2023-12-28/future-trajectory-gold-prices-2024-2026-navigating-economic-and-geopolitical)
