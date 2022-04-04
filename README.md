# Australia state level Covid-19 Policy Responses
Systematic dataset of Australian sub-national Covid-19 policy data

**NOTE:** for Australian subnational data that is directly comparable with our country-level data, please visit our [OxCGRT/covid-policy-tracker](https://github.com/OxCGRT/covid-policy-tracker) repository.

This is a project from the [Blavatnik School of Government](https://www.bsg.ox.ac.uk) in collaboration with the [Australian National University](https://www.anu.edu.au/)  drawing on the [Blavatnik School of Government OxCGRT](https://www.bsg.ox.ac.uk/covidtracker).

More information is available on the project's website: [https://www.bsg.ox.ac.uk/research/research-projects/coronavirus-government-response-tracker](https://www.bsg.ox.ac.uk/research/research-projects/coronavirus-government-response-tracker).

---

### Dataset of Australian sub-national Covid-19 government response policies

Drawing on the Oxford COVID-19 Government Response Tracker (OxCGRT) [coding system](https://github.com/OxCGRT/covid-policy-tracker/blob/master/documentation/codebook.md), we provide a systematic and objective account of the strength of Covid-19 response policies that have been instigated by Australia’s federal government and state and territory governments.  

Currently we provide coding for 16 indicators: C1 through C8, E1, E2 H1 through H3, and H6 through H8. These indicators allow the creation of four different [indices](https://github.com/OxCGRT/covid-policy-tracker/blob/master/documentation/index_methodology.md): the stringency index, the containment and health index, the government response index and economic support index. The dataset is updated continuously in real time. 

### Differences between the levels of policies 

This repo contains data for three levels of policies, described using the suffixes of "GOV", “WIDE”, and “TOTAL”. Policies described with the suffix "GOV" refers to policies issued only at a specific level of government. 

Policies described with the suffix “_WIDE” capture all government responses set by a given jurisdiction and its sub-components. “_WIDE” policies do not incorporate general policies from higher levels of government that may supersede local policies, but they do capture policies from higher-level governments if they are specifically targeted at that subnational jurisdiction. For example, if a national government orders events to close in a particular city experiencing an outbreak. Policies described with the suffix “TOTAL” describe all government responses taken by a specific jurisdiction, those below it , and also includes inherited policies from higher levels that affect that jurisdiction. For example, if a country has an international travel restriction that applies country-wide, this would appear as a NAT_GOV policy and be inherited by STATE_TOTAL and CITY_TOTAL, but not by STATE_WIDE nor CITY_WIDE. 

The AUS subnational repo contains eight descriptive labels: 

- NAT_GOV: Policies issued by the Australian federal government only. 
- NAT_TOTAL: Part of the OxCGRT international dataset, describes the overall policy environment that applies to residents of the country, including policies set by the subnational governments where those values are more stringent than country-wide action. 
- STATE_GOV: Policies issued by that particular state government only. 
- STATE_WIDE: Describes government responses set by a state and its sub-components. It does not include policies adopted at a higher level of government. 
- STATE_TOTAL: Describes the overall policy environment that applies to residents of the state, including policies set by the national government where those values are more stringent than state-level action. 
- CITY_GOV: Policies that affect that particular ‘city’ only within the jurisdiction e.g. policy affecting Greater Sydney or Rest of NSW. In Australia, the city either refers to the state’s greater capital city or the rest of the state. 
- CITY_WIDE:  For Australia, health policies are not implemented by city officials and consequently CITY_WIDE is the same as CITY_GOV. 
- CITY_TOTAL: Describes the overall policy environment that applies to residents of the city, including policies set by the national government and state government where those values are more stringent than city-level action.


### Further interpretation

Flags representing distinctions between targeted/general measures for subnational data products are consistent with those in the existing OxCGRT [codebook](https://github.com/OxCGRT/covid-policy-tracker/blob/master/documentation/codebook.md). 

### Getting data from this GitHub repository

The [/data](data/) folder in this repo contains recent exports from the OxCGRT database. You are welcome to build applications that draw directly from this repository. The data is a full export from the database presented in "state-day" format, with a column of notes from our data collectors for each indicator. This is updated manually on a regular basis, and so the file name may change. Please note that some of the comments contain commas and other characters interpreted as a delimiter, and so may cause problems when parsing this CSV file.

### Acknowledgments

The OxCGRT Australian subnational coders are:
