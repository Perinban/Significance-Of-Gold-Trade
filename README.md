SIGNIFICANCE OF GOLD TRADE ON BRICS VS OTHER NATIONS


# Table of Contents {#table-of-contents .TOC-Heading}\

[1) Abstract:\
[2) Introduction:\
&emsp;[2.1) What is BRICS?\
&emsp;[2.2) Why are BRICS nations formed?\
&emsp;[2.3) What is BRICS currency?\
&emsp;[2.4) Impact on US Dollars by BRICS Currency\
[3) Methods:\
&emsp;[3.1) Data Preprocessing:\
&emsp;&emsp;[3.1.2) Data Analysis:\
&emsp;&emsp;[3.1.3) Data Transformation:\
&emsp;&emsp;[3.1.4) Data Mean Substitution:\
&emsp;&emsp;[3.1.5) Data Outliers Handling:\
&emsp;&emsp;[3.1.6) Data Validation:\
&emsp;&emsp;[3.1.7) Data Readiness:\
&emsp;[3.2) Other Data Sources:\
[4) Exploratory Analysis:\
&emsp;[4.1) Trade Value between countries for each Quartiles:\
&emsp;[4.2) Net Weight between countries for each Quartiles:\
&emsp;[4.3) Analysis on Gold Trade Value:\
&emsp;[4.4) Analysis on Gold Purchase Quantity:\
&emsp;&emsp;[4.4.1) Why UAE Stopped purchasing Gold in 2021?\
&emsp;&emsp;[4.4.2) Why Canada Started buying Gold in 2019?\
&emsp;&emsp;[4.4.3) Why Switzerland bought more gold from Kenya than Egypt?\
&emsp;[4.5) Why South Africa has lesser Partners when compared to Others?\
&emsp;[4.6) Why some countries pay less price than world bank price?\
&emsp;[4.7) Why UAE stopped buying gold by Egypt and starts to buy from other countries?\
&emsp;[4.8) Comparative Analysis of South Africa's Gold Imports: Kenya vs Other Countries\
[5) Gold Purchase Forecast BRICS VS Other Countries\
[6) Conclusion\
[7) References\
[8) Appendix

# 1) Abstract:

This research provides the importance of gold trade imports from the
reporting countries such as South Africa, Kenya and Egypt focusing on
relation between the BRICS countries and other nations. This analysis
completely relies on the data from the UN ComTrade database on the
periods from 2017 to 2023 which signifies the pre-covid, covid and
post-covid of gold trade data between countries. This study evaluates
various data methodologies on the gathered data to make it readiness for
meaningful insights and help the experts to understand how gold has been
influencing the markets around the world. Gold has become a prominent
way of trade without the use of US dollars, and this study explores how
the BRICS nations are conducting this trade worldwide which paves the
way for emerging the new currency. These findings assess how this new
currency becomes the revolutionary and grows fast among the countries
for trade around the world. The insights on various trends over the
volume and price helps the professionals understand why there is a
sudden change in the market in recent years. Gold Trade on various years
has been performed from various directions understanding how prominent
the market evolved currently and helps the countries grew fast more
economical. This also considers on how the dominant countries fall and
offers more meaning forecasting insights about the future.

Keywords: Gold trade, UN Comtrade, BRICS nations, Emerging Currency,
Market Analysis, Trend Analysis, Price, Quantity, Import, Export, South
Africa, Kenya and Egypt

# 2) Introduction:

This study explores the impact on the US dollar resulting from gold
trade exports between BRICS countries and other nations. This focuses on
reporters such as South Africa, Kenya, and Egypt data that are readily
available to us. The data has been sourced from the UN ComTrade
database, via API with frequent data updates. Since the data has taken
from free version with certain parameters which consists of aggregated
results to a certain degree (AGGR_LEVEL = 4/6) rather than open bulk
data. This makes the data less accurate and faulty results. Hence, to
make quality of the content, this study does not consider any historical
or future predictions of the data and consider only the current data
from 2017 to 2023. That covers the periods such as before, during, and
after COVID-19, with each period span of two years. Due to the
limitations of the free version of the UN ComTrade data, additional data
handling methods were used to get proper analysis results.

# 2.1) What is BRICS?

BRIC is known for Brazil, Russia, India, China which is formed in 2009,
and in 2010 the South Africa was added, forming five major economics in
the world. The concept of BRICS is proposed in 2001 by Jim O'Neill, and
the first official meeting which is held by five nation leaders
Yekaterinburg Russia in 2009 and in December 2010 south Africa was
invited to join the group then the name changes from BRIC to BRICS,
which enhance its geopolitical influence \[1\]**.**

# 2.2) Why are BRICS nations formed?

The BRICS nations aim to grow their economy by co-operation, mutual
trade and mutual investment. The key objective of formation was to
reform the international financial institutions like World bank and
International Monetary Fund (IMF) which is dominated by western nations
\[2\].

# 2.3) What is BRICS currency?

The concept of BRICS currency has been circulated around the five
nations such as Brazil, Russia, India, China and South Africa. The main
objective of the BRICS currency is to create and promote a new financial
system in gold trade among global markets. The evolution of new BRICS
currency will reduce the usage of US dollar in the global gold trade. In
recent days, trade system has been evolved to reach its peak of 100% by
prominent US dollars which paved the way for United states to influence
the global financial systems.

The BRICS currency is backed by the pool of five nation currencies which
is Brazilian Real, Russian Ruble, India Rupee, Chinese Renminbi, and
South African Rand which refers to R5 or R5+ currency \[3\] and this
idea includes a backing element in the form of commodities such as Gold
to promote additional security for the new currency \[4\].

There is no sign of implementations of the BRICS currency yet, but the
process of evolution continues to grow and gets updated in the future
BRICS summits. The main theme of 2023 summit was to discuss on
upbringing the BRICS currency, but it has not been released yet.

# 2.4) Impact on US Dollars by BRICS Currency

As of now the traditional method to trade international transactions are
held in US Dollars. In the year 2023, the BRICS nations discussed about
creating new currency that are backed by gold paving the way to the
evolution of BRICS currency. This BRICS currency will completely change
the global transactions trade which is held in US dollars. As a first
step, BRICS are introducing a new currency by masking "de-dollarization"
which will impact enormously on US dollars.

The US dollars is prominent as world primary reserves for decades. This
process of de-dollarization is complex; to bring it in effect as the
BRICS need the reliable payment systems by considering all the problems
that may arise as the BRICS nations continues towards de-dollarization
to decrease the dependence on US dollars \[5\].

The economic consequences for the United States will make impact on
economic adjustments within the United States. The main advantage of
this BRICS currency to reduce the conversion costs for the trade among
the member nations more efficiently \[6\].

# 3) Methods:

The research on the gold trade exports has been conducted with the
various techniques and methods such as below:

# 3.1) Data Preprocessing:

The source data has been processed based on the data wrangling
techniques such as below:

# 3.1.1) Data Availability:

The source data for this research has been taken from the UN ComTrade
database. The data has been obtained from source through the API by
passing the below parameters:

> *Freqcode = M* #Monthly
>
> *ClsCode = HS* #HS Classification
>
> *Period = 2017 to 2023*
>
> *ReporterCode = 404, 710, 818* #Kenya, South Africa, Egypt
>
> *CmdCode = 7108, 710811, 710812, 710813, 710820* #Gold
>
> *FlowCode = X* #Export

# 3.1.2) Data Analysis:

Based on the "Mapping Document.xlsx" workbook \[mentioned in Appendix
1\], data analysis has been conducted to the access data via API calls
and the data has been filtered based on given criteria mentioned under
"Assumptions" column in "Mapping" Sheet. The raw source data extracted
via API is archived in the data lake table named as "GOLD_TRADE_DL"

# 3.1.3) Data Transformation:

For certain attributes with similar values, data transformation has been
performed so that the final records contain only non-zero/non-null
values for the mandatory columns and sent for further processing. Below
are the conditions listed for the transformation:

i.  **Primary Value:** This attribute defines the trade value in
    dollars. The records with the trade value such as blank, or null
    values are considered as invalid. In such conditions, the
    corresponding value is copied directly from the FOB_VALUE, as
    FOB_VALUE contains exact export values.

ii. **Net Weight:** This attribute defines the trade volume in
    kilograms. The records with the trade volume such as blank, or null
    values are treated as invalid. In such cases, data has been compared
    with Qty and AltQty attributes. If the value is in grams, data has
    been converted and then copied to NetWeight in Kilograms as we are
    dealing with only grams and kilograms data from the source.

# 3.1.4) Data Mean Substitution:

For certain records, we have identified that the data has been missing
or as 0 for the required attributes. In such cases, to avoid loss of
data, data has been filled with mean values from the other months for
the reporters which makes the data consistent while plotting for
visualization.

# 3.1.5) Data Outliers Handling:

As we are dealing with the real-time data with combination of reported
and aggregated values, there is a high possibility that data may fall on
invalid range which makes the visualization inconsistent. To avoid such
issues, z-score outliers has been performed by calculating the relation
between the important attributes and then those records are removed
which makes the data ready for visualization.

# 3.1.6) Data Validation:

After analyzing the data, there are lot of duplicates found on basis of
aggregated values. To clean those duplicate sum values, data validation
has been performed using "Data Validation.xlsx" \[mentioned in Appendix
2\]. Records that fail to satisfy the conditions are rejected and stored
in the reject table named as "GOLD_TRADE_DATA_REJECT ". Records that met
the conditions are stored in the data warehouse table named as
"GOLD_TRADE", with the final columns listed in the requirement document.

# 3.1.7) Data Readiness:

To visualize the data, not all the attributes mentioned in the
requirement specifications are required. Hence, unwanted attributes are
removed and are stored in the data mart table named as
"GOLD_TRADE_DATA_MART".

# 3.2) Other Data Sources:

Historical standard gold prices for comparison are collected from world
bank \[7\], then converted from oz to the kilograms and stored in the
table named "GOLD_PRICE".

Information that are related to the BRICS countries are sourced from
Wikipedia \[8\] and then updated with Partner data taken from ComTrade,
stored in the table named "BRICS_CONT".

# 4) Exploratory Analysis:

This research has been analyzed with various trends based on volume and
price such as below:

# 4.1) Trade Value between countries for each Quartiles:

![A screenshot of a graph Description automatically
generated](./media/image2.png){width="6.425365266841645in"
height="3.4179724409448817in"}

Based on the data availability, it is showed that that the United Arab
Emirates has constantly purchasing the gold in dollars each year across
quartile. However, some countries have not made gold trade more than a
million.

In year 2017, United Arab Emirates has purchased over \$459M in Q1 for
purchasing gold who stands at the top, followed by Switzerland with
\$131M, Turkey with \$59M and Lebanon with \$65M. Due to the high
purchases of gold in Q1 reduces their buying in subsequent quartiles due
to the dynamic market fluctuations.

In 2020, United Arab Emirates spent over \$524M in Q3 on gold trade
which stands the highest on all data. This was followed by Canada and
Australia in buying more gold for different quartiles. Multiple
countries have shown their interest in the recent years to buy more gold
and countries who purchased before could not continue due to the
financial instability and economic crises.

# 4.2) Net Weight between countries for each Quartiles:

![A diagram of a company Description automatically generated with medium
confidence](./media/image3.png){width="6.400049212598425in"
height="3.4399825021872266in"}

Based on the data availability, we can interpret that the South Africa
has been consistently acquiring large volumes of gold over the years for
all different quartiles. However, some countries have not even purchased
for about 1000 kilograms.

In 2017, South Africa has imported gold of about 101K in first quartile,
followed by 75K in third quartile, 58K in second quartile and 46K in
fourth quartile. Followed by South Africa, Switzerland has purchased
about 51K in third quartile which is the highest among all its
quartiles. The United Arab Emirates acquired about 12K in the first
quartile, followed by 11K in fourth quartile and 10K in second quartile.

In the year 2020, South Africa predominately acquired 114K of gold in
fourth quartile and 58K in the first quartile. The United Arab Emirates
has purchased around 10K in first quartile, followed by 13K in second
quartile and 6K in fourth quartile.

However, countries like United Arab Emirates, who spent significantly on
gold trade acquired only lesser amount of gold, but South Africa who
spent very less money, have attained more gold of them all. This was due
to the changing market standards change and new methods adaption by
trading other products as compensation.

# 4.3) Analysis on Gold Trade Value:

![A graph showing the value of a period Description automatically
generated](./media/image4.png){width="6.388888888888889in"
height="4.138888888888889in"}

Gold Trade has reached its peak on 2020 with 2.9 billion due to the
COVID-19 pandemic. But unfortunately, there is a significant drop in
2021 with 1.1 billion as investors have found the better source with
good returns than gold \[9\].

The United States economy appears unstable, as the manufacturing sector
were weakened as goods orders fell by 2% in November. Consumer spends
that drives the economy of about 70% is heavy on debt. The Federal
government continues to lower interest rates to sustain from this debt,
but it could not be able to last indefinitely. Due to this, investors
are seeking golds as a safe place \[10\].

Russia leads the trend by mining operations producing 185 tons of gold
which is about 18% increase from 2018. This has indicated that Russia's
gold reserves have shifted away from the U.S. dollars. This trend has
mirrored by rich people and central banks globally, thus increasing gold
holdings. This makes the gold price increase in the upcoming years.

As the gold prices increase, individuals are finding a safer place with
lower interest where they get better returns which makes them to go away
from gold from 2021.

# 4.4) Analysis on Gold Purchase Quantity:

![A graph with lines and numbers Description automatically
generated](./media/image5.png){width="6.388888888888889in"
height="3.9770833333333333in"}

Gold trade has increased on the year 2020 due to the COVID-19 pandemic
which makes the market volatile and economically instable. Investors
around the world has considered gold as a safe-haven asset and purchased
more which made its price go up. The governments and central banks have
taken significant actions to avoid economic impact during pandemic, that
there would be chances of inflation, currency weakening, which in turn
has increased the demand for gold. Central banks have also reduced the
interest rates nearly zero, to create an opportunity for the people of
holding assets like gold\[11\].

As the COVID-19 vaccines were started to roll out, countries have
started to recover economically, investors have migrated their purchases
from gold to stocks. As people anticipated economic recovery and higher
inflation, they made fixed income investments than gold. In 2021, the US
dollar has reached its peak making gold more expensive for people with
other currencies to buy. As inflation made the price go high, central
banks have taken measures to raise increase rates which made gold less
attractive during inflation.

# 4.4.1) Why UAE Stopped purchasing Gold in 2021?

![A graph showing the price of a gold purchase Description automatically
generated](./media/image6.png){width="5.2004965004374455in"
height="3.2373097112860894in"}

In 2021, the United Arab Emirates has stopped purchasing gold due to the
increasing inspection over the illegal trade from African Countries.
There were a lot of gold smuggling takes place over the zones in Africa,
which makes the global countries had thought that their money from the
trade has been used for criminal activities. The United Arab Emirates
has denied that they are not involved in illegal activities, but
international groups and governments has teased Dubai's gold market for
not doing enough to stop the smuggling. This has hurt Dubai's reputation
a lot, which made Dubai to make more stricter rules and monitoring to
avoid these issues in the future \[12\].

# 4.4.2) Why Canada Started buying Gold in 2019?

![A graph of a line graph Description automatically generated with
medium confidence](./media/image7.png){width="5.121797900262467in"
height="3.188320209973753in"}

The Canada has decided to buy gold in 2019 due to the economic
uncertainties, looking for different reserves, and they found gold as a
stable and safeguard against the inflation and currency fluctuations
\[13\]. This helps them to broaden their trends among the central banks
and institutional investors globally during that period. However, in
2016 they have liquidated all their gold reserves, and some finance
report said that the government has retained around 77 ounces \[14\].

The trade war between US and China has created economic uncertainty,
making investors and countries to check for safer assets. Due to the
change in global market's instability and frequent changes in the market
conditions made gold a more attractive option. As global demand for gold
rises due to reduced risks, Canada has decided to buy gold same as other
countries and institutions to defend their reserves and protect against
market up and down.

In 2022, Canada has sold their gold reserves due to the change in
Canadian dollar, which was traded with low 70 cents to the US dollar,
compared to the value same as 2010 and 2014. Along with the rising oil
prices, transportation issues, and stabilize the real estate market has
made the Canadian dollars go high. Factors that affect gold prices are
interest rates, the US dollar, and risk sensitivity, and the global
demand for jewelry and geopolitical uncertainties \[15\]. Since 2016,
due to the low interest rates and uncertainty towards market, countries
have adapted themselves to buy gold which increased gold demand. The
future of the gold prices will completely depend on factors like oil
price, market stability, and global economic conditions.

# 4.4.3) Why Switzerland bought more gold from Kenya than Egypt?

![A map of the world with different countries/regions Description
automatically generated](./media/image8.png){width="6.388888888888889in"
height="4.029166666666667in"}

Compared to Egypt, Switzerland imports more gold from Kenya. This
development can interface to number of components that influence
exchange flow, such as generation capacity, administrative
administrations, showcase openness, and verifiable exchanging
associations.

Kenya is as it were one of the African countries with whom Switzerland
has built solid financial ties. It is conceivable that Kenya\'s
endeavors to create its mining industry and exchange organization have
expanded and openness to Swiss gold merchants. Switzerland, which is
well-known for its sizable gold refining division, as often as possible
looks for trustable and successful gold providers. Kenya might exchange
more with Switzerland, have a greater affect over the mining segment,
and utilize more proficient send out procedures \[16\].

Kenya may have pulled in Swiss buyers of gold since of its strong
legitimate and regulatory system. To development around the world trade
and wander, Kenya has been bracing its mining laws. For countries like
Switzerland, where steady and straightforward financial ties are basic,
these administrative changes may move forward the commercial climate.
Swiss buyers may dishearten from managing with Egyptian gold trades as
much on the off chance that Egypt\'s regulatory obstructions are more
exorbitant & complicated

Although Kenya has as of late expanded its yield of gold, Kenya may have
opened modern markets for Swiss dealers. Egypt, on the other hand,
contains a solid capacity to create gold. From 50,000 units in 2017 to
488,847 units in 2023, Kenya\'s gold sends out expanded significantly,
illustrating a speedy rise.

This development might give Switzerland with a new and critical supply
of gold, fitting well with their needs. Besides, the mining division in
Kenya can give competitive estimating or superior conditions that suit
the financial interface of Switzerland.

Current arranging framework as well as important exchange designs are
attractive. It is conceivable that Switzerland has way better set up
commercial associations and understandings with Kenya than with Egypt,
which makes bringing in gold from Kenya less demanding strategically and
more reasonable.

For superior business-related associations, steady administrative
systems, Kenya\'s extending generation capacity, effective planning, and
the country\'s seen soundness are the most reasons for Switzerland\'s
current inclination for gold imports from Kenya over Egypt. All these
components combined make Kenya a more alluring and reliable exchange
accomplice for imports of Swiss gold.

# 4.5) Why South Africa has lesser Partners when compared to Others?

![A screenshot of a chart Description automatically
generated](./media/image9.png){width="6.388888888888889in"
height="3.736111111111111in"}

From 1905 to 2007, South Africa has been the one of the top best gold
sellers and it has mined 30% of the gold mining around the word.
However, after this, it has started to decline due to the many reasons,
such as expensive techniques must be employed to get the deeper gold as
below \[17\]:

-   Decline in Gold Production:

<!-- -->

-   Depletion of Reserves: Due to the excessive mining, high-grade gold
    reserves have been significantly depleted. Remaining reserves that
    are available on the deeper underground makes the extraction more
    difficult and expensive.

-   Operational Costs: The cost of mining has been increased gradually
    due to the technological advancement and deeper mining operations
    which makes the profits less in gold production.

<!-- -->

-   Labor and Social Issues:

<!-- -->

-   Labor Disputes: In the mining sector, gold production operations
    have been disrupted enormously due to the labor strikes and constant
    disputes raised among them.

-   Working Conditions: Due to the harsh and dangerous working
    conditions in the deeper underground mines, South Africa has made
    less productivity and increased ethical concerns.

<!-- -->

-   Illegal Mining and Crimes:

<!-- -->

-   Illegal Mining: Illegal mining activities such as zama zamas has
    caused more disruptions. Also, these illegal mining operations are
    associated with violence, crime and making the working conditions
    unsuitable.

-   Organized Crime: Criminal organizations have increased rapidly on
    the mining industry, which leads to various issues such as human
    trafficking and exploitation.

<!-- -->

-   Regulatory and Political Challenges:

<!-- -->

-   Corruption: Due to the increased corruption in the mining tender
    evaluation and enforced regulatory environment, companies are afraid
    to invest in production that makes mining industry an unstable and
    unattractive environment.

-   Regulatory Environment: Due to the frequent regulatory and policy
    changes such as environmental protection and labor rights makes the
    mining process increase their operational costs.

<!-- -->

-   Economic Factors:

<!-- -->

-   Fluctuating Gold Prices: Gold prices have fluctuated constantly due
    to the US dollars that affects the profits margin of gold mining
    processes. Mining companies without any marginal profit makes them
    hard to mine and sell gold.

-   Global Competition: As there is an ongoing greater competition with
    the other gold producing countries such as China, Australia and
    Russia, South Africa has been rough due to the less mining
    conditions and less production levels when compared to them.

<!-- -->

-   Environmental and Social Concerns:

<!-- -->

-   Environmental impact: Due to the strict law enforcements and
    increased awareness on the mining activities in companies, they
    suffer with increased costs and operational constraints from
    government.

-   Community Impact: Effects on local communities on the mining
    activities has led to the increased pressure to make sure the
    process is sustainable, and all the ethical practices are followed
    strictly.

# 4.6) Why some countries pay less price than world bank price?

![A screenshot of a graph Description automatically
generated](./media/image10.png){width="5.1393974190726155in"
height="2.9280949256342956in"}

Some countries pay less than the World Bank\'s quoted gold price due to
the local market conditions such as excess supply or lower demands. This
also lowers local prices compared to the global market and fluctuates
the local currency values against the US dollar led to variations in
gold prices. Costs that are associated with importing or exporting gold,
includes tariffs, customs taxes and transportations costs which
finalizes the trade price. Government policies and subsidies, such as
lower tax on gold purchases can make the gold cheaper domestically.
Interferences in the market and uncertain behavior can cause differences
between local and global prices. Illegal mining and smuggling affect the
pricing of gold in certain regions as black-market gold does not any
additional costs and regulation policies. Trade barriers and economic
conditions also influences pricing costs as in certain areas have less
access for buyers to gold. Finally, variations in gold quality and
purity creates multiple change in price differences such as lower purity
gold sold for less price.

# 4.7) Why UAE stopped buying gold by Egypt and starts to buy from other countries?

![A graph of the year Description automatically generated with medium
confidence](./media/image11.png){width="6.268055555555556in"
height="3.8361111111111112in"}

During the first five months of 2023, gold exports from Egypt has
decreased to approximately 45% due to reduction in the global demand and
falling gold prices. This makes the investors to move towards the better
attractive investments that are suitable for them to sustain other than
gold. Additionally, Egypt has not evolved their marketing standards to
adapt new technological advancements rather following old traditional
methods. The UAE\'s demand for Egyptian gold had fell sharply from \$442
million to \$110 million in 1 year. In Egypt, high demand for gold has
been influenced by inflation and falling Egyptian pound which makes it
very hard to export gold domestically. Raising interest rates make the
investors look for the investments more attractive than gold, leading
the UAE to look for other sources \[18\].

# 4.8) Comparative Analysis of South Africa's Gold Imports: Kenya vs Other Countries

![](./media/image12.png){width="6.388888888888889in"
height="4.084722222222222in"}

This study is to look at the patterns and amount of gold trade from 2017
to 2023 between Kenya and its main trading partners (South Africa,
Switzerland, and the United Arab Emirates). By data analysis, the report
emphasizes Kenya\'s expanding significance as a gold supplier to South
Africa and Switzerland, its plays a key involvement in the gold trade.

For the economy of African nations, including Kenya, the gold trade is
vital. Trade policy and economic strategies may be ongoing thorough an
understanding of the amount and patterns of gold imports and exports.
The dynamics of Kenya\'s gold trade--- its dealings with South Africa,
Switzerland, and the United Arab Emirates. It also analyzes the reasons
behind Switzerland\'s decision to import more gold from Kenya rather
than Egypt.

We used extensive trade data from reliable sources to examine the
patterns in the gold trade between Kenya and its main trading partners,
South Africa, Switzerland, and the United Arab Emirates, from 2017 to
2023. The following were the main data sources like UN ComTrade Database
Pie charts were used to graphically represent the data, making it clear,
how much gold was exchanged between Kenya and its partner nations in
2023. The net weight of gold imported from Kenya by South Africa and
Switzerland was shown.

The annual trade volumes from 2017 to 2023 have been calculated using
patterns based on data. The approximate annual figures are shown below:
An examination of the gold trade between Kenya and its main trading
partners, South Africa, Switzerland, and the United Arab Emirates, from
2017 to 2023, might yield significant data on current trends in the gold
market.

Gold shipments from Kenya to South Africa have increased significantly,
according to trade statistics the years 2017 to 2023. South Africa rose
to become the world\'s largest importer of gold from Kenya, rising from
50,000 units in 2017 to 488,847 units by 2023. This remarkable rise can
be attributed to several factors: More strong trade agreements between
Kenya and South Africa have likely increased business\'s profit and ease
of doing business. This has resulted in strengthened bilateral relations
\[19\].

Major developments in the gold mining industry have increased as per
Kenya\'s ability to produce and export gold. Kenya is a major provider
of gold since South Africa is a big player in the gold market. The main
import of gold from Switzerland, which has developed from 25,000 units
in 2017 to 184,339 units in 2023. Gold must meet strict quality and
purity criteria, and Switzerland is known for having these standards.
Kenya gold may more reliably satisfy these demanding requirements than
gold from other sources. The consistent rise points to dependable and
stable commercial ties between Kenya and Switzerland, underpinned by
advantageous trade arrangements and circumstances.

# 5) Gold Purchase Forecast BRICS VS Other Countries

![A graph showing the price of a company Description automatically
generated with medium
confidence](./media/image13.png){width="6.388888888888889in"
height="4.057638888888889in"}

Based on the data collected from 2017 to 2023, BRICS countries has
purchased the gold at the average of \$52,877 per kilogram on 2023,
while the other countries purchased the gold at the average of \$42,515
per kilogram on 2023. The data has been forecasted for the next 3 years
to check how the data will look on the future trends.

From the forecasting results, it is estimated that BRICS countries are
expected to purchase the gold at the average cost of \$56,100 on 2024,
\$59,467 on 2025 and \$62,384 on 2026. Other countries are estimated to
purchase the gold at the average cost of \$39,090 on 2024, \$40,963 on
2025 and \$42,836 on 2026 \[20\].

In the forecasted data, it is clearly shown that BRICS countries are
ready to pay more to buy more gold as they are on the way to introduce
their own currency that are backed by gold. This helps them to reduce
the usage of US dollar soon for trade by replacing with their own BRICS
currency. The higher average purchase indicates the importance on
building strong gold reserves, as a foundation for economic stability
against dynamic global environmental changes.

![A screenshot of a report Description automatically
generated](./media/image14.png){width="4.690770997375328in"
height="2.9771106736657917in"}

Based on the summary results, it is predicted that the BRICS countries
could purchase at the peak increase of 12.0%, while the other countries
could see peak purchase increase of 9.6%. This indicates the strong
relation of gold acquisition for the BRICS countries when compared to
the other countries.

# 6) Conclusion

The study explores the importance of gold trade exports between BRICS
and other countries in US dollars, using data gathered for South Africa,
Kenya and Egypt. Based on UN ComTrade database, we analyzed data from
2017 through 2023 and identified various trends to understand the key
insights behind those periods.

Our findings reveal that the BRICS countries have purchased gold to
bring down the US dollars so that they can bring their own currency
backed with gold, which ensures stable trade among member nations
without conversion charges.

The forecasted data indicates that the BRICS countries are willing to
pay higher prices of gold, to build their new system. This helps them
building a better currency for the replacement of the US dollars.

In summary, this study evaluates why the importance of gold for BRICS
nations and how they bring forward their new currency. This highlights
the ongoing studies to understand implications of gold trade and
economic stability.

# 7) References:

1)  <https://www.goldmansachs.com/intelligence/archive/building-better.html>

2)  <https://www.cfr.org/expert-brief/how-brics-got-here>

3)  https://moderndiplomacy.eu/2022/12/21/a-brics-reserve-currency-exploring-the-pathways/

4)  <https://www.chards.co.uk/guides/brics-summit-2023-is-the-gold-backed-digital-currency-coming/1198>

5)  <https://www.lowyinstitute.org/the-interpreter/de-dollarisation-shifting-power-between-us-brics>

6)  <https://www.policycircle.org/opinion/brics-currency-faces-challenges/>

7)  <https://thedocs.worldbank.org/en/doc/5d903e848db1d1b83e0ec8f744e55570-0350012021/related/CMO-Historical-Data-Monthly.xlsx>

8)  <https://en.wikipedia.org/wiki/Member_states_of_BRICS>

9)  <https://www.forbes.com/sites/kenroberts/2021/04/30/with-1-billion-monthly-surplus-us-gold-trade-shaking-off-wild-2020/>

10) https://www.ccn.com/5-key-reasons-why-golds-price-is-set-to-skyrocket-in-2020/

11) [Is gold a hedge or a safe-haven asset in the COVID--19
    crisis?](https://pdf.sciencedirectassets.com/271681/1-s2.0-S0264999321X00077/1-s2.0-S0264999321001772/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEOn%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJHMEUCIE6OP1oH%2BGBFhG51v%2FSm8hmJO5P21BEW55RHu%2F21H60MAiEAlgVi%2FGugXjdDwJz%2F7KGp6mKV3pXuTiIw5dn3qD4dMF4qvAUIwf%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAFGgwwNTkwMDM1NDY4NjUiDDRMUQpV9CDR5ZbLpyqQBTr0LRfVWutn40UVi7MaYjnqaoyL8CLqgiyyDDU8JJ70%2B0om2%2Fs%2BwgF155R80g4XIf9ewDWWGpkNeWmHREH6TcbAhQi%2BQcmpepKVUXCdczrs2EFAeqTy%2B86c1EbKRILe96VK%2BIARFd9DBydJxqqeRgp7Dko3FXe7aIqJG%2B5euKubkOr7BtcugKpNO1MMJSdpP4010m4RGJa0Og%2Bum6CNGq8yok2%2FN54V%2BnVRv7oUKiQfJH7hJkz0beV2f3Gz66rH8632s9a5n2jVMDhzgiJIQ%2ByqgnsFXtIRhEgsLboAISmNO4HmV5D1HLGogKLrOFBCcNbYKx0QbUS14LcMVcrAyMbMKFfpnZBcdVQYTn3gErmhYtZF%2Bz5t%2BzJOSLELfj16IIKYq75H6hvdyaGc9qM9knrrkpJNZOidck7H8BHcWkCZfnO7ScKklx4YuOOaupNwiKZHunOcT1Ls1P0IBYUDF5L6SeJCiLshogb9HDLhfD5wH5QAYNZcAeyeLZms%2Bns7aut2emwSofhXPrxzSBoJWArisvLkIIjeNI7rDjX3wjh2KCGspXUWVjxnZmjoRu30blWCe1m%2FNZLqiXMN414M9arm8sWQtzEpdrvQnJpvBCHVZzQ5RAyonmFEQ0UtzUf%2BdImk3Osr%2BGKVVhaUct%2BbSgCh8LaGXXjh2%2BR1mBYgcWeYE669PSHY0oBVKrd2Cmc70qXluPwxSIv9FbY8kQ5gcEokbnciiP8nLen4bf6NMbvFEQTjcfW8DQiVe6NpY%2FWlx8vDztMC6Yr%2FM1JIe0IanVkyGVAuCZQLS%2F6V%2FYK5YVdDZBZvXkavqsVyNmNr63CRYTeJFw2nke2D%2F%2BKVxXA5zPz%2FtFB5agJUWSLk7rBY323QMILwibUGOrEBRnFVZt%2Fk7d5yM%2BiZJlfKUZrXQXWdO0q9MTeBi3l%2Bdhrk%2BZslOJCDk1zdgiUUVTiUSALzO%2BwnBHwCDJ6pp99VyxNy7l0bPNfgnorUoI39SIEU4Qz0SuY2PuRxoc7Wm0mNeDe5WMp0RO2uV%2F7%2FW7H8ylTLswCis3GwKJ6jHaG6ysJQpfGda4RNoQ5uCjj8FhXrQDvfu%2FuUPFTY9pFRCUgBr9Yv00Gn7l3LtD%2BSciWPXlkH&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20240725T162916Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTYYU7P6AXS%2F20240725%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=7df126aef29f99804369aae613c42ab8e230a787d9289753abe5df7efa7af61a&hash=a4c1e7d95bf4da8bac54ac5168c5b793101cc1f35246caaaa301fc0ea814f20a&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0264999321001772&tid=spdf-675fe4bc-cab2-4e9b-99fc-c18b53c2933a&sid=a4f692cc5d48344e724916e-2e40f00b53)

12) <https://www.bloomberg.com/news/features/2021-12-28/where-does-gold-come-from-in-africa-suspected-smuggling-to-dubai-rings-alarms>

13) <https://financialpost.com/commodities/mining/chinas-zijin-mining-agrees-to-buy-canadas-continental-gold-for-about-1-bln>

14) [[https://tradeimex.in/blogs/switzerland-gold-trade-import-export-statistics-of-2023]{.underline}](https://tradeimex.in/blogs/switzerland-gold-trade-import-export-statistics-of-2023)

15) <https://www.cbc.ca/news/business/gold-canada-reserves-1.3475818>

16) <https://www.forbes.com/advisor/money-transfer/usd-cad-forecast/>

17) <https://www.corruptionwatch.org.za/delving-into-the-shady-world-of-gold-laundering/>

18) <https://www.dailynewsegypt.com/2023/07/16/egypts-gold-exports-decline-by-45-in-5m-2023/>

19) <https://www.the-star.co.ke/news/2023-01-11-where-kenya-south-africa-should-start-to-address-trade-barriers/>

20) <https://www.kitco.com/opinion/2023-12-28/future-trajectory-gold-prices-2024-2026-navigating-economic-and-geopolitical>

# 8) Appendix:

  --------------------------------------------------------------------------
    **Document Name* **Details**                                **Reference
                                                                 Number**
  ------------------ ----------------------------------------- -------------
       Mapping       This document contains the data analysed        1
    Document.xlsx    as part of assumptions and analysis       
                     performed                                 

         Data        This document includes the data with            2
    Validations.xlsx validation steps and rejections           

    Source Code.ipynb This file contains the Python source code       3
                     of data extraction, data cleansing, data  
                     loading to tables, data rejection         
                     processes, etc                            

       Database      This file contains the queries used for         4
      Tables.sql     creating tables that are part of this     
                     research                                  

      Brics.xlsx     This document contains the data gathered        5
                     from Wikipedia and converted to required  
                     format to be used for this research       

     Gold Price.xlsx This document contains the data gathered        6
                     from world bank and converted from oz to  
                     kilograms to be used as part of this      
                     research                                  

    GoldTrade.twbx   This file contains the tableau                  7
                     visualisation charts that are built as    
                     part of this research                     
  --------------------------------------------------------------------------
