# 🌍Global-Oil-and-Gas-Analysis

# 📚Table of Content

[Project Overview](#project-overview)

[Data Sources](#data-sources)

[Tools and Technologies](#tools-and-technologies)

[Data Preparation](#data-preparation)

[Data Overview](#data-overview) 

[Tabular Overview](#tabular-overview) 

[Objective](#objective)

[Analysis Visualization](#analysis-visualization)

[Key Insights](#key-insights)

[Actionable Recommendations](#actionable-recommendations)


## 📌Project Overview

This project presents a structured analysis of global oil and gas production, pricing, and export values across 187 countries over the period 1932–2014. The analysis was carried out to evaluate long-term energy trends, export value concentration, and population-adjusted economic impact.

The work focuses on understanding how oil and gas markets have evolved over time, identifying countries that dominate global exports, and assessing the relationship between energy value and national population size. 
The project translates complex, multi-decade energy data into clear analytical insights that support strategic decision-making in energy economics, policy planning, and investment analysis. 


## 🧩Data Sources

The primary dataset used for this analysis  was sourced from “Kaggle.com”


## 🛠Tools and Technologies

1. Power BI – Data modeling, visualization, and interactive dashboards

2. Excel – Data cleaning, transformation, and validation

3. DAX – Measures, aggregations, and calculated metrics

## ⚙🧹Data Preparation

In the initial data cleaning phase, the following tasks were performed:

## 🧾Data Overview 

 🔹Geographic Coverage: 187 countries
 
 🔹Time Span: 1932–2014
 
The dataset includes the following columns:

**🟥Country** 

🔹Country_Name – Official country name

🔹ISO3 Numeric – ISO numeric country code

🔹Country_id – Internal country identifier

🔹Year – Year of observation

🔹EIA_cty_name – Country name as used by the EIA


**🟧Oil Metrics**

🔹Oil_prod32_14 – Oil production volume

🔹O il_price_2000 – Oil price indexed to year 2000

🔹Oil_price_nom – Nominal oil price

🔹oil_value_nom – Nominal oil production value

🔹oil_value_2000 – Oil production value (2000 constant prices)

🔹oil_value_2014 – Oil production value (2014 constant prices)


**🟨Gas Metrics**

🔹gas_prod55_14 – Gas production volume

🔹gas_price_2000_mboe – Gas price per barrel equivalent (2000 prices)

🔹gas_price_2000 – Gas price indexed to year 2000

🔹gas_price_nom – Nominal gas price

🔹gas_value_nom – Nominal gas production value

🔹gas_value_2000 – Gas production value (2000 constant prices)

🔹gas_value_2014 – Gas production value (2014 constant prices)


**🟩Combined Oil & Gas Value**

🔹oil_gas_value_nom – Nominal oil and gas value

🔹oil_gas_value_2000 – Oil and gas value (2000 constant prices)

🔹oil_gas_value_2014 – Oil and gas value (2014 constant prices)


**🟦Per-Capita Oil & Gas Value**

🔹oil_gas_valuePOP_nom – Nominal oil and gas value per population

🔹oil_gas_valuePOP_2000 – Per-capita oil and gas value (2000 prices)

🔹oil_gas_valuePOP_2014 – Per-capita oil and gas value (2014 prices)


**🟪Oil Trade**

🔹oil_exports – Total oil exports

🔹net_oil_exports – Oil exports minus imports

🔹net_oil_exports_mt – Net oil exports (metric tonnes)

🔹net_oil_exports_value – Value of net oil exports

🔹net_oil_exports_valuePOP – Net oil export value per population


**🟫Gas Trade**

🔹gas_exports – Total gas exports

🔹net_gas_exports_bcf – Net gas exports (billion cubic feet)

🔹net_gas_exports_mboe – Net gas exports (barrel oil equivalent)

🔹net_gas_exports_value – Value of net gas exports

🔹net_gas_exports_valuePOP – Net gas export value per population


**⬛Combined Trade & Demographics**

🔹net_oil_gas_exports_valuePOP – Net oil & gas export value per population

🔹population – Total population

🔹pop_maddison – Population estimate (Maddison Project)


**⬜Metadata & Conversions**

🔹sovereign – Sovereign state indicator

🔹mult_nom_2000 – Nominal-to-2000 price conversion factor

🔹mult_nom_2014 – Nominal-to-2014 price conversion factor

🔹mult_2000_2014 – Price conversion factor (2000 to 2014)



## Tabular Overview 

A brief overview of raw tabular datasets to be analyzed. The first 5 Columns are displayed below.

Country_Name|	ISO3 Numeric|	Country_id|	Year|	EIA_cty_name|	Oil_prod32_14|	Oil_price_2000	|oil_price_nom|	oil_value_nom|	oil_value_2000|	oil_value_2014|	gas_prod55_14|	gas_price_2000_mboe|	gas_price_2000|	gas_price_nom|	gas_value_nom|	gas_value_2000|	gas_value_2014|	oil_gas_value_nom|	oil_gas_value_2000|	oil_gas_value_2014|	oil_gas_valuePOP_nom|	oil_gas_valuePOP_2000|	oil_gas_valuePOP_2014|	oil_exports|	net_oil_exports|	net_oil_exports_mt|	net_oil_exports_value|	net_oil_exports_valuePOP|	gas_exports|	net_gas_exports_bcf|	net_gas_exports_mboe|	net_gas_exports_value|	net_gas_exports_valuePOP|	net_oil_gas_exports_valuePOP|	population|	pop_maddison|	sovereign|	mult_nom_2000|	mult_nom_2014|	mult_2000_2014|
|----|----|-----|----|----|----|----|-----|----|----|----|----|-----|----|----|----|----|-----|----|----|----|----|-----|----|----|----|----|-----|----|----|----|----|-----|----|----|----|----|-----|----|----|----|
Afghanistan|	4	|AFG	|1932	|Afghanistan	|0	|10.86086|	0.87|	0	|0	|0	|0	|0	|	0.06|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	| |	|	1	|12.599874|	17.32197312|	1.374773519|
Afghanistan|	4	|AFG	|1933|	Afghanistan|	0|	8.815239|	0.67|	0|	0|	0	|0	|0	|	0.06|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	| |	|		1	|13.280064	|18.25708032|	1.374773519|
Afghanistan	|4	|AFG	|1934	|Afghanistan	|0|	12.71579|	1	|0	|0	|0	|0	|0	|	0.06	|		|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	| |		|1	|12.853008|	17.66997504|	1.374773519|
Afghanistan	|4	|AFG	|1935	|Afghanistan	|0|	12.03969|	0.97|	0|	0|	0	|0	|0	|	0.06|		|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	| |	|	1|	12.537882|	17.23674816|	1.374773519|
Afghanistan	|4	|AFG	|1936	|Afghanistan	|0	|13.38321	|1.09	|0	|0	|0	|0	|0	|	0.06|		|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	|	| |		|	1	|12.420786	|17.07576768|	1.374773519|




## 🎯Objective

 ✒  Analyze oil and gas production trends across countries

 ✒ Compare export values and prices over time

 ✒  Identify top oil and gas exporting countries

 ✒ Evaluate per-capita export value to understand real economic impact

 ✒ Deliver actionable insights using data visualization and storytelling



## 🎨Analysis Visualization

Chart Analysis 


## 📈Key Insights

### EXCEL ###

1. Average Oil Production by Year
   
*Insights*:

◻ There is a strong long-term upward trend in average oil production, indicating sustained growth in oil extraction over the years.

◻Production accelerated significantly after the early years, suggesting major discoveries, technological improvements, or increased investment.

◻In recent years, oil production appears to plateau, implying possible market maturity, production caps, or regulatory constraints.


2. Average Gas Production by Year
   
*Insights*:

◻Gas production shows a gradual increase initially, followed by a steeper growth phase, reflecting rising global demand for natural gas.

◻Short-term fluctuations indicate market sensitivity, likely influenced by price volatility, infrastructure expansion, or geopolitical factors.

◻Overall trend confirms gas as a growing complementary energy source to oil.


3. Standard Deviation of Oil Prices (Base Year 2000)
   
*Insights*:

◻Oil price volatility remains relatively low and stable in earlier years.

◻Sharp spikes in standard deviation during certain periods indicate high market instability, often linked to:
Global economic crises
Supply shocks
Geopolitical conflicts

◻Recent spikes suggest that oil prices have become increasingly unpredictable, increasing financial risk for producers and exporters.


4. Top 10 Net Oil Export Value Revenue by Country
   
*Insights*:

◻Saudi Arabia dominates global oil export revenue, confirming its position as a leading oil exporter.

◻Russia and Iran follow closely, highlighting their strong dependence on oil exports for national revenue.

◻Countries like Nigeria, UAE, and Norway show substantial earnings, indicating oil remains a major contributor to their economies.

◻Revenue concentration among few countries suggests global oil supply is highly centralized.


5. Top 10 Gas Export Value Revenue by Country
   
*Insights*:

◻Russia leads gas export revenues by a wide margin, reinforcing its influence in the global gas market.

◻Canada and Norway are strong secondary exporters, reflecting advanced gas infrastructure and export capacity.

◻Countries such as Qatar and Australia highlight the growing importance of LNG (Liquefied Natural Gas) exports.

◻Gas export revenue is more geographically diversified compared to oil.


6. Top 10 Net Oil & Gas Exports Value per Population (Average)
   
*Insights*:

◻Qatar and Brunei rank highest, indicating extremely high export revenue relative to population size.

◻Smaller nations with large reserves show higher per-capita benefits from oil and gas exports.

◻Larger countries like Saudi Arabia generate high absolute revenue but lower per-capita values due to population size.

◻This highlights how oil and gas wealth can have disproportionate economic impact in smaller economies.

### POWER-BI ###

1. Overall Data Coverage - REWRITE
   
This dashboard analyzes oil and gas performance across 187 countries over a long historical period (1932–2014).

This wide coverage allows us to see global patterns, not just trends in a few oil-rich nations.

3. Average Oil Production
   
Oil production is very high on average, clearly showing that oil has been the dominant energy resource globally for decades.

Many countries have relied heavily on oil for energy supply and export revenue, making oil a major driver of national economies.

4. Average Gas Production
   
Gas production is lower than oil but still significant and steadily present across many countries.

This suggests that gas has played a supporting and growing role, especially as countries diversify their energy mix.

5. Oil & Gas Value vs Price (Year 2000)
   
Countries with strong production still earn heavily, even when prices fall.

7. Top Oil & Gas Exporting Countries (Total Value)

Russia and the United States lead by a wide margin.

Saudi Arabia remains one of the most influential oil exporters globally.

This shows that global energy supply is concentrated, making the market sensitive to disruptions in these key countries.

8. Oil Export Value: 2000 vs 2014
   
Average oil export value increased noticeably from 2000 to 2014.

Overall, oil remained a strong revenue generator during this period.

9. Gas Export Value: 2000 vs 2014
    
Gas export value also shows clear growth over time, similar to oil.

This indicates that gas is becoming increasingly valuable, supported by:

Expansion of gas infrastructure

Growing demand for cleaner energy sources


10. Net Oil & Gas Export Value per Population

Smaller countries like Qatar and Brunei benefit the most per person.

Larger countries earn more in total but less per person due to population size.

This highlights that resource wealth impacts citizens differently, depending on population and revenue management.

## 💰Actionable Recommendations

### EXCEL

1. Reduce Dependence on Crude Oil Revenue

Diversify national income by investing in downstream oil activities such as refining and petrochemicals.

Channel oil revenues into non-energy sectors to minimize exposure to oil price volatility.


2. Prioritize Natural Gas as a Growth Driver

Expand gas infrastructure including LNG terminals and processing facilities.

Position natural gas as a transition fuel in long-term energy strategies.


3. Mitigate Oil Price Volatility Risks

Implement price hedging mechanisms and long-term supply contracts.

Establish or strengthen stabilization and sovereign wealth funds to manage revenue shocks.


4. Optimize Production Efficiency

Shift from production expansion to efficiency-driven optimization using advanced extraction technologies.

Reduce operational costs through process automation and predictive maintenance.


5. Improve Per-Capita Economic Impact in Large Exporting Countries

Reinvest export earnings into education, infrastructure, and industrial development.

Promote domestic energy utilization to support job creation and economic growth.


6. Diversify Energy Export Markets

Expand exports to emerging and regional markets to reduce geopolitical risk.

Develop long-term bilateral energy trade agreements.


7. Ensure Long-Term Sustainability for High Per-Capita Exporters

Invest surplus revenues into future-focused industries and sovereign wealth funds.

Implement fiscal policies that reduce overdependence on energy exports.


8. Adopt Continuous Data Monitoring and Forecasting

Leverage analysis to track production trends, price volatility, and export performance.

Integrate forecasting models to support proactive decision-making.

### POWERBI

◻Reduce over-reliance on crude oil by investing in downstream processing) and non-oil sectors to manage price volatility risks.

◻Scale natural gas development by expanding LNG, processing, and pipeline infrastructure to capitalize on its steady growth and cleaner energy role.

◻Strengthen revenue risk management through price hedging, long-term supply contracts, and stabilization or sovereign wealth funds.

◻Optimize production efficiency as oil output matures by focusing on cost reduction, automation, and advanced extraction technologies.

◻Diversify export markets to reduce geopolitical exposure and improve long-term revenue stability.

◻Improve per-capita economic impact by reinvesting oil and gas revenues into education, infrastructure, and industrial development.

◻Adopt continuous data monitoring and forecasting using BI tools to support proactive, data-driven energy policy decisions.


💻 📊


