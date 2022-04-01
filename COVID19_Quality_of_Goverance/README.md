# covid-19-and-quality-of-governance
Preliminary analysis of the influence of quality of governance on COVID-19 vaccinations

<b>Data Sources:</b>
- The source for the COVID-19 Vaccination dataset can be found here: https://www.kaggle.com/gpreda/covid-world-vaccination-progress, which consists of data collated from here: https://github.com/owid/covid-19-data/tree/master/public/data/vaccinations. 
- The source for the Quality of Governance dataset is the World Bank and can be found here: https://info.worldbank.org/governance/wgi/. 

Access to both datasets in this project is free and open to the public and does not violate any laws.

<b>Context:</b>

As more people in the US receive COVID vaccinations, the lack of vaccinations in other parts of the world becomes more and more apparent and concerning. We should wonder why some countries have made more progress than others in terms of delivering vaccines to their populations. To address this, the specific goal for this project is to examine the impact of a country's quality of governance on the amount of vaccines it has administered so far. 

<b>What is quality of governance?</b> For the purposes of this analysis, quality of governance is essentially how well a country runs. The dataset used here captures six world governance indicators (WGI):
   1. <b>Voice and Accountability</b>: Reflects perceptions of the extent to which a country's citizens are able to participate in selecting their government, as well as freedom of expression, freedom of association, and a free media.
   2. <b>Political Stability and Absence of Violence</b>: Measures perceptions of the likelihood of political instability and/or politically-motivated violence, including terrorism.
   3. <b>Government Effectiveness</b>: Reflects perceptions of the quality of public services, the quality of the civil service and the degree of its independence from political pressures, the quality of policy formulation and implementation, and the credibility of the government's commitment to such policies.
   4. <b>Regulatory Quality</b>: Reflects perceptions of the ability of the government to formulate and implement sound policies and regulations that permit and promote private sector development.
   5. <b>Rule of Law</b>: Reflects perceptions of the extent to which agents have confidence in and abide by the rules of society, and in particular the quality of contract enforcement, property rights, the police, and the courts, as well as the likelihood of crime and violence.
   6. <b>Control of Corruption</b>: Reflects perceptions of the extent to which public power is exercised for private gain, including both petty and grand forms of corruption, as well as "capture" of the state by elites and private interests.
   
I want to ask the question: <b>Does the amount of vaccines delivered to people differ based on a country's quality of governance, according to a given indicator?</b>
   
Estimates for a country for any given WGI range from -2.5(weak governance) to 2.5 (strong governance). Estimates are designed to be normally distributed about 0. More on the methodology for calculating these WGIs can be found here: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=1682130. 

<b>Previous Research/Analyses:</b>
- Dataset 1 Global COVID Vaccinations: there have been several analyses done using this dataset that explore what country-level factors correlate with vaccinations. These range from public health expenditure, GDP, etc., but do not look at indicators of quality of governance. 
- Dataset 2 World Governance Indicators: there have been a couple of analyses that try to examine the effect of governance on COVID-19 mortality and COVID-19 policy responses, but none that compare governance and vaccination progress. 

<b>Hypothesis:</b>

My previous experiences in political science/international relations research qualify me to conduct this analysis, and <b>I hypothesize that countries with better governance are able to deliver more vaccines to their populations</b>. Through the analysis, we should be able to see which, if any, governance indicators are more relible signals of this hypothesized trend. 

<b>Data Overview:</b>

Prior to processing, the COVID Vaccination dataset is 3.1 MB with 15666 rows and 15 columns. The World Governance Indicator dataset is 1.8 MB with 216 rows and 128 columns. 
