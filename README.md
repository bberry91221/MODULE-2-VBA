![Gemsolar_mind-blowing_installation.PNG](Resources/Gemsolar_mind-blowing_installation.PNG)

Gemasolar is a concentrated solar power plant with a molten salt heat storage system. It is located within the city limits of Fuentes de Andalucía in the province of Seville, Spain and generates enough power for 27,500 households per year.
The above image is an example of the newest form of energy being developed currently. Investors hungry for high producing stocks is the funding source for the research and development being done by ground-breaking solar energy companies like this one. For information about this solar power plant that was dedicated in October 2011: [Gemasolar](https://en.wikipedia.org/wiki/Gemasolar_Thermosolar_Plant).


# MODULE-2-VBA: Stock Analyses using VBA Excel Macro


## I. Overview of Project
Steve's parents have been investing since 2017 in a "green" company that they felt was the best investment. Steve, on the other hand, is not certain that they had all the facts at hand to make a good determination. He asked for help in analyzing whether their investment plan was appropriately set on the best company which would give the highest rate of return over time. The company Steve's parents chose has the NYSE ticker or stock symbol "DQ" (DAQO New Energy Corp.). They had chosen this company because it produces "green" energy which they are highly interested in. Their goal is to support sustainable energy sources that do not affect the environment negatively. To broaden Steve's parent's perspectives, it was not enough to just compare DQ's returns for 2017 and 2018. Calculating the stock performance by using the annualized Total Return will show the financial gain (or loss) in their stock price. Another indicator of general investor interest is to compare the Total Volume, i.e., the number of stocks traded per year. Taking this analysis further, collecting this information for all 11 remaining companies will lend a good comparison, especially if these companies also share production of similar solar products and equipment. Using this data for both 2017 and 2018 will depict a more broad picture of the growth potential for solar energy products across all 12 companies, including DQ.


## II. Results
As mentioned above, there are three characteristics we will be analyzing across all 12 companies:
    1. The Total Return of the stocks was collected daily and included in the provided database. Taking each price at the opening of trading and subtracting the ending price at the end of the day was compiled across the entire year for each stock. This number was converted to a percentage and placed in the tables below for each year showing the gains (cell background is green) and losses (cell background is red) for each company. 
    2. Also, the other charactertistic we focused on was on the Total Volume of trades summed up by each company for each year to mark the interest in the investor pool out in the general, potential stockholders' public.
    3. We also wished to see the performance of the macros by 2 methods of calculation used, i.e., running the calculations linearly (calculating each company's numbers, one at a time) and using a method with embedded arrays to calculate each characteristic all at once across all 12 companies. 


### A. How the Analyses Were Completed: Daily Closing Stock Prices

We collected stock prices across 12 solar energy companies for 2 years (2017 and 2018). The calculations to obtain the Annual Return were based on subtracting the Closing price from the previous day from the Closing stock price from the current day of trading for each of these years. Here is the portion of the macro code which calculated these numbers (Note: there is an index counter at play in order to keep track of each days' calculations. Also, the hard-coded "6" is actually where the Closing prices are located in the database.)

![how_to_calculate_annual_return_per_stock.PNG](Resources/how_to_calculate_annual_return_per_stock.PNG)

The results are listed below and are augmented by cell background colors to quickly show GAINS (green cells) and LOSSES (red cells). From the years 2017 and 2018 for the 12 companies, you can see in these tables that 2017 was a banner year for solar power companies. Almost all of the companies enjoyed a positive total return on shareholders' stocks. 

![2017_Calc_Return.PNG](Resources/2017_Calc_Return.PNG)<img height="350" hspace="20"/>![2018_Calc_Return.PNG](Resources/2018_Calc_Return.PNG)

The table below gives the ticker names, full names of companies and top 3 highest returns in this list.  

| Return % | Rank | Ticker | Full Company Name |
|----------|------|--------|--------------------|
| | | AY |Atlantica Sustainable Infrastructure |
|   |   | SIQ | Canadian Solar Inc. |
| 199.4% | #1 | DQ | DAQO New Energy Corp.|
| 129.5% | #3 | ENPH |Enphase Energy Inc.|
| | | FSLR | First Solar Inc.|
| | | HASI | Hannon Armstrong Sustainable Infrastruture Capital Inc.|
| | | JKS  | JinkoSolar Holding Co. Ltd.|
| | | RUN  |SunRun Inc.|
| 184.5% | #2 | SEDG |SolarEdge Techologies, Inc.|
| | | SPWR |SunPower Corp.|
| | | TERP |TerraForm Power Operating, LLC|
| | | VSLR |Vivint Solar|


As mentioned above, we further investigated the huge returns. This fact begs the question about what was happening business-wise that would cause 11 out of 12 solar energy companies to post such high gains. For the top 3 companies, this information was found online and is paraphrased below:

For the "wide" view of stock performance, "Renewable energy once again achieved record increases in capacity in 2017," (from [Green_Tech_Media.com](https://www.greentechmedia.com/articles/read/2017-another-record-busting-year-for-global-renewable-energy-capacity). From another, well-respected source, REN21 is the only global renewable energy community of scientists, governments, NGOs and industrial experts providing insights into the need of renewable energy. They provide up-to-date and peer-reviewed facts, figures and analysis of global developments in technology, policies and markets. Their goal is to enable decision-makers around the world to make the shift to renewable energy happen – now before it is too late. from: [REN21](https://www.ren21.net/about-us/who-we-are/)


**#1 - "DQ" (Daqo New Energy Corp.)** is a Chinese company engaged in the manufacture of monocrystalline silicon and polysilicon, primarily for use in solar photovoltaic systems. The company operates a mono-Si and poly-Si manufacturing facility located in Shihezi, Xinjiang Province, China. ... DAQO formerly manufactured silicon wafers at a facility in Chongqing, China (discontinued in 2018) from: [DQ Wikipedia Pages](https://en.wikipedia.org/wiki/Daqo_New_Energy).

**#2- SEDG (SolarEdge Technologies, Inc.)** is an American Israeli provider of power optimizer, solar inverter and monitoring systems for photovoltaic arrays.These products aim to increase energy output through module-level Maximum Power Point Tracking (MPPT).[2] Established in 2006, the company has offices in the United States,[3] Germany,[4] Italy, Japan, and Israel. In May 2015, SolarEdge partnered with Tesla Motors[9] for the joint development of a photovoltaic (PV) storage and backup power solution for the residential solar market, based on the Powerwall home and industrial battery packs that were unveiled in April 2015,[10] and quickly received orders to a total value of US$800 million. In October 2018, SolarEdge announced agreements to acquire a major stake in Kokam, a South Korean provider of Lithium-ion battery cells, batteries and energy storage solutions. Using SolarEdge's direct current (DC) optimized inverter and Tesla's automotive-grade battery technology, the solution requires only a single SolarEdge inverter to manage both PV and storage functions. The system is designed for efficient, outdoor installation and includes remote monitoring and troubleshooting to keep operations and maintenance costs low. In October 2020, SolarEdge has partnered with Schneider Electric. This alliance is planned to provide a cohesive electricity environment for installers and device owners, while also accelerating solar installation experience across the region. from https://en.wikipedia.org/wiki/SolarEdge.

**#3 - ENPH (Enphase Energy Inc.)** is an American NASDAQ-listed energy technology company headquartered in Fremont, California. Enphase designs and manufactures software-driven home energy solutions that span solar generation, home energy storage and web-based monitoring and control. Enphase has shipped about thirty million solar microinverters, primarily into the residential and commercial markets in North America, Europe and Australia. [3] Microinverters convert the direct current power from the solar panel (DC) directly into grid-compatible alternating current (AC) for use or export.[4] Enphase was the first company to successfully commercialise the microinverter on a wide scale, and remains the market leader in their production. 2017 began the introduction of the new IQ architecture, which uses a new cabling system. Two conductors, down from four, are integrated and compliant with electrical codes due to the use of GFCI, no need for a neutral and no conductive materials in the enclosure. The initial products were the IQ6 and IQ6+, followed in 2018 by the IQ7. In 2019 the IQ8 series will enable continuous power production during grid outages during daytime without the need for batteries. from: https://en.wikipedia.org/wiki/Enphase_Energy

The lowest performing stock that registered actual losses was **TERP (Terraform)** which is the only company that is not wholly providing equipment or components for solar power. 

This company is a subsidiary of SunEdison which has had financial troubles (including having to file for Chapter 11) since April 2016. In July 2017, the U.S. Bankruptcy Court approved SunEdison's bankruptcy-exit plan and it eventually emerged from bankruptcy December 29, 2017. "TerraForm Power is a global renewable energy project development company. It owns and operates solar and wind generation assets serving utility, commercial, and residential customers. It owns and operates over 200 solar power projects. Its scope extends to other clean power generation such as natural gas, geothermal, hydro-electricity, and hybrid power generation." from https://en.wikipedia.org/wiki/SunEdison

## Summary - TO DO: In a summary statement, address the following questions.
What are the advantages or disadvantages of refactoring code?
How do these pros and cons apply to refactoring the original VBA script?

There is a detailed statement on the advantages and disadvantages of refactoring code in general (3 pt).
There is a detailed statement on the advantages and disadvantages of the original and refactored VBA script (3 pt).


There are very clear choices that will, based on the last 2 years of data, produce a nice return for Steve's parents.

 11 other companies with a similar business focus, i.e., implementation and innovation of solar panel components.


## Results 
We collected stock prices across 12 solar energy companies for 2 years (2017 and 2018). The returns were calculated by using the Closing stock price for each day of trading for each of these years. Here is the portion of the macro code which calculated these numbers.
![how to calculate annual return per stock.PNG](Resources/how to calculate annual return per stock.PNG)

Also, we were able to sum up the Total Daily Volume for each stock on days of trading for 2017 and 2018. Please see the finished tables below showing the annual return as well as the Total Daily Volume for each stock. Please note the stocks that are colored green. This means the return had increase through the year. The red cells show a loss in the price of the stocks.
![2017_Calc_Return.PNG](Resources/2017_Calc_Return.PNG)  ![2018_Calc_Return.PNG](Resources/2018_Calc_Return.PNG)


'''''''ut in Subheadings too.IS DQ a good company to invest in? Daqo dropped over 63% in 2018—yikes! Steve will definitely want to offer some better stocks to his parents.
The macro compiled for these tables used an array of values, meaning that the calculations for the returns as well as the Total Volume were calculated at the same time while running through the code. This is a more efficient way of running any code that has many lines of numbers. Each year had prices and Volumes for all 3,012 stocks. In looking at the time it took to execute the code for 2017, it took over 77 seconds. For 2018, it took over 74 seconds. See below.
![VBA_Challenge_2017.PNG](Resources/VBA_Challenge_2017.PNG)  ![VBA_Challenge_2018.PNG](Resources/VBA_Challenge_2018.PNG)

It should be much lower than these figures so I took the opportunity to run this same code on a brand new laptop and turned off all memory-hogging applications (like these 2 browsers: Chrome and Edge browser; plus I temporarily turned off Norton Antivirus program which necessitated disconnecting any network connection(s) as well). The results are listed below.

GET NEW TIMERS
ALSO GET execution times of the ORIGINAL script 

We used stock prices from the years 2017 and 2018 for the following 12 companies, including "DQ":

**AY**-Atlantica Sustainable Infrastructure
CSIQ-Canadian Solar Inc.
DQ-DAQO New Energy Corp. 199.4% return! 2017
ENPH-Enphase Energy Inc. 129.5% 2017
FSLR-First Solar Inc.
HASI-Hannon Armstrong Sustainable Infrastruture Capital Inc.
JKS-JinkoSolar Holding Co. Ltd.
RUN-SunRun Inc.
SEDG-SolarEdge Techologies, Inc. 184.5% return 2017
SPWR-SunPower Corp.
TERP-TerraForm Power Operating, LLC
VSLR-Vivint Solar

"Renewable energy once again achieved record increases in capacity in 2017" quoted from a report from the Renewable Energy Policy Network of the 21st Century (REN21), a policy organization with members across national governments, industry and divisions of the United Nations. REN21 provides knowledge about what is happening now in the renewable energy sector and how the latest trends will impact future developments. from https://www.ren21.net/about-us/what-we-do/

Below are the tables depicting the Total Annual Volume and overall return calculated for the year for each company's stock.
![VBA_Challenge_2017.PNG](Resources/VBA_Challenge_2017.PNG) ![VBA_Challenge_2018.PNG](Resources/VBA_Challenge_2018.PNG)

In this graph (Source: https://www.google.com/search?q=atlantica+sustainable+infrastructure+plc+stock&sxsrf=APq-WBsx9Pk3vkUVogaCOnGMLp49fqeDew%3A1647181884785&source=hp&ei=PAAuYpqkLMmeptQPt7W2gAE&iflsig=AHkkrS4AAAAAYi4OTBRuPJeoEQYFQm6dnoTJ_R41MUz_&oq=Atlantica+Sustain&gs_lcp=Cgdnd3Mtd2l6EAEYAzILCC4QgAQQxwEQ0QMyCggAEIAEEIcCEBQyBQgAEIAEMgUIABCABDIFCAAQgAQyBQgAEIAEMgUIABCABDIFCAAQgAQyBQgAEIAEMgUIABCABDoECCMQJzoRCC4QgAQQsQMQgwEQxwEQ0QM6DgguEIAEELEDEMcBENEDOgsILhCABBDHARCjAjoICC4QsQMQgwE6EQguEIAEELEDEMcBEKMCENQCOgsILhCABBCxAxCDAToLCC4QgAQQsQMQ1AI6DgguEIAEELEDEMcBEKMCOhEILhCABBCxAxDHARCvARDUAjoICC4QgAQQsQM6CAgAEIAEELEDOgsIABCABBCxAxCDAToLCC4QsQMQxwEQowI6BQguEIAEOggIABCxAxCDAToLCC4QsQMQxwEQ0QM6CwguEIAEEMcBEK8BOg0ILhCABBDHARDRAxAKOggIABCABBDJA1AAWKsfYI1CaABwAHgAgAGoAYgB3g2SAQM5LjiYAQCgAQE&sclient=gws-wiz, you can see AY stock performance up to yesterday. The 2 years we have figures for show prices at around $19.

For information about this concentrated solar power plan with a molten salt heat storage system (dedicated in October 2011): https://en.wikipedia.org/wiki/Gemasolar_Thermosolar_Plant

DON't include: Canadian Solar Inc. is a publicly traded company that manufactures solar PV modules and runs large scale solar projects (from: https://en.wikipedia.org/wiki/Canadian_Solar)

### 2017 RETURNS: TOP 3 SOLAR COMPANIES
#1 highest return (199.4%) across all 12 companies examined herein. DAQO (DAQO New Energy Corp.) is a Chinese company engaged in the manufacture of monocrystalline silicon and polysilicon, primarily for use in solar photovoltaic systems. The company operates a mono-Si and poly-Si manufacturing facility located in Shihezi, Xinjiang Province, China. DAQO formerly manufactured silicon wafers at a facility in Chongqing, China (**discontinued in 2018**). (from: https://en.wikipedia.org/wiki/Daqo_New_Energy)

#2 highest return (184.5%) across all 12 companies examined herein. SEDG (SolarEdge Technologies, Inc.) is an American Israeli provider of power optimizer, solar inverter and monitoring systems for photovoltaic arrays. These products aim to increase energy output through module-level Maximum Power Point Tracking. (from: https://en.wikipedia.org/wiki/SolarEdge)

#3 highest return (129.5%) across all 12 companies examined herein. ENPH (Enphase Energy) is an American NASDAQ-listed energy technology company headquartered in Fremont, California. Enphase designs and manufactures software-driven home energy solutions that span solar generation, home energy storage and web-based monitoring and control. They were also "the first company to successfully commercialise the microinverter on a wide scale, and remains the market leader in their production today". (from: https://en.wikipedia.org/wiki/Enphase_Energy)

### 2018 RETURNS: TOP 3 SOLAR COMPANIES

#1 highest return (84.0%) across all 12 companies examined herein. RUN (Sunrun Inc.) is an American provider of residential solar panels and home batteries, headquartered in San Francisco, California. In July 2018, Sunrun expanded their solar and battery service to the island of Puerto Rico. With operations in 23 states, the District of Columbia, and Puerto Rico, Sunrun became the largest solar, storage and energy services company in America, surpassing Solar City. (from https://en.wikipedia.org/wiki/Sunrun) As seen in the table, RUN had the third highest Total Daily Volume at 1.5 trillion stocks.

#2 highest return (81.9%) across all 12 companies examined herein. Enphase Energy in 2017 began the introduction of the new IQ architecture, which uses a new cabling system. Two conductors, down from four, are integrated and compliant with electrical codes due to the use of GFCI, no need for a neutral and no conductive materials in the enclosure. The initial products were the IQ6 and IQ6+, followed in 2018 by the IQ7. In 2019 the IQ8 series will enable continuous power production during grid outages during daytime without the need for batteries." (from: https://en.wikipedia.org/wiki/Enphase_Energy) As seen in the table, ENPH had the highest Total Daily Volume at 1.83 trillion stocks.

SolarEdge shows a 7.8% drop in their returns for 2018. Impacting their business plans was the announcement in October 2018 agreements to acquire a major stake in Kokam, a South Korean provider of Lithium-ion battery cells, batteries and energy storage solutions.

These 2 companies had the only positive returns in comparison against the other solar power companies.

NEED SUBHEADING
IS DQ a good company to invest in? Daqo dropped over 63% in 2018—yikes! Steve will definitely want to offer some better stocks to his parents.

## Summary
There are very clear choices that will, based on the last 2 years of data, produce a nice return for Steve's parents.

What are the advantages or disadvantages of refactoring code?
How do these pros and cons apply to refactoring the original VBA script?

There is a detailed statement on the advantages and disadvantages of refactoring code in general (3 pt).
There is a detailed statement on the advantages and disadvantages of the original and refactored VBA script (3 pt).

