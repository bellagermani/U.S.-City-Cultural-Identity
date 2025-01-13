# U.S. City Cultural Identity
This jupyter notebook imports data from multiple sources, cleans, merges, and exports a final dataset that will be used to examine the relationship between various cultural aspects of U.S. cities and their innovation outputs.



### Data:
The unit of study is Metropolitan Statistical Area (MSA)

Each variable in the final dataset includes values between 2010 & 2015 only.


### Variables:
Num Cult Estab = Number of cultural establishments present per every 100,000 people (NOT INCLUDED IN FINAL DATASET- not enough availability over time)

- Source: NADAC Local Arts Index (https://www.icpsr.umich.edu/web/NADAC/studies/36984#) 

<br/>

Percent Emp = Percent of population working in the Arts, Entertainment, & Recreational industries. Constructed from Total Employment & AER Employment

&nbsp;&nbsp;&nbsp;&nbsp;Total Employment = Total number of people employed

- &nbsp;&nbsp;&nbsp;&nbsp;Source: Bureau of Economic Analysis Regional Data - GDP and Personal Income (https://apps.bea.gov/itable/ReqID=70&step=1#eyJhcHBpZCI6NzAsInN0ZXBzIjpbMSwyOSwyNSwzMSwyNiwyNywzMF0sImRhdGEiOltbIlRhYmxlSWQiLCIzMyJdLFsiTWFqb3JfQXJlYSIsIjUiXSxbIlN0YXRIixbIjUiXV0sWyJBcmVhIixbIlhYIl1dLFsiU3RhdGlzdGljIixbIjEwIl1dLFsiVW5pdF9vZl9tZWFzdXJlIiwiTGV2ZWxzIl0sWyJZZWFyIixbIi0xIl1dLFsiWWVhckJlZ2luIiwiLTEiXSxbIlllYXJRW5kIiwiLTEiXV19)

&nbsp;&nbsp;&nbsp;&nbsp;AER Employment = Total number of people employed in the Arts, Entertainment, & Recreational industries

- &nbsp;&nbsp;&nbsp;&nbsp;Source: Bureau of Economic Analysis Regional Data - GDP and Personal Income (https://apps.bea.gov/itable/?ReqID=70&step=1#eyJhcHBpZCI6NzAsInN0ZXBzIjpbMSwyOSwyNSwzMSwyNiwyNywzMF0sImRhdGEiOltbIlRhYmxlSWQiLCIzMyJdLFsiTWFqb3JfQXJlYSIsIjUiXSxbIlN0YXRlIixbIjUiXV0sWyJBcmVhIixbIlhYIl1dLFsiU3RhdGlzdGljIixbIjE3MDAiXV0sWyJVbml0X29mX21lYXN1cmUiLCJMZXZlbHMiXSxbIlllYXIiLFsiLTEiXV0sWyJZZWFyQmVnaW4iLCItMSJdLFsiWWVhcl9FbmQiLCItMSJdXX0=)

<br/>

Fborn Pop = Total number of foreign-born people in the population

- Source: Census Bureau S0502 - Selected Characteristics of the Foreign-Born Population by Period of Entry Into the United States (https://data.census.gov/table/ACSST5Y2022.S0502?g=010XX00US$31000M1)

<br/>

Percent Speak Other Lang = Percent of people who speak a second language

- Source: Census Bureau S1601 - Language Spoken at Home (https://data.census.gov/table/ACSST5Y2022.S1601?g=010XX00US$31000M1)

<br/>
 
Perc GDP = The percentage of GDP that originates from Arts, Entertainment, Recreational, Performance, Museums, and Spectator Sports

- Source: Bureau of Economic Analysis Gross Domestic Product by Metropolitan Area (https://apps.bea.gov/histdatacore/HistFileDetails.html?HistCateID=2&FileGroupID=41)

<br/>

Pat = Total number of utility patents produced

- Source: U.S. Patent & Trademark Office - Patenting In Technology Classes Breakout by Origin, U.S. Metropolitan and Micropolitan Areas (https://www.uspto.gov/web/offices/ac/ido/oeip/taf/cls_cbsa/allcbsa_gd.htm)

<br/>

Pop = Total Population (control)

- Source: Bureau of Economic Anslysis Regional Data - GDP and Personal Income - CAINC30 Economic profile (https://apps.bea.gov/itable/?ReqID=70&step=1#eyJhcHBpZCI6NzAsInN0ZXBzIjpbMSwyOSwyNSwzMSwyNiwyNywzMF0sImRhdGEiOltbIlRhYmxlSWQiLCIxMiJdLFsiTWFqb3JfQXJlYSIsIjUiXSxbIlN0YXRlIixbIjUiXV0sWyJBcmVhIixbIlhYIl1dLFsiU3RhdGlzdGljIixbIjEwMCJdXSxbIlVuaXRfb2ZfbWVhc3VyZSIsIkxldmVscyJdLFsiWWVhciIsWyItMSJdXSxbIlllYXJCZWdpbiIsIi0xIl0sWyJZZWFyX0VuZCIsIi0xIl1dfQ==)
