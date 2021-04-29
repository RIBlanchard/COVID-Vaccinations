# COVID-Vaccinations
Forecasts number of people fully vaccinated in the US using vaccinations from Our World in Data and Bass diffusion model.

Assumption: market size (m) is set to US population; an enhancement to this analysis would estimate fraction of population that will get vaccinated and adjust m.

Steps:
1. Load data from owid/covid-19-data
2. Aggregate to weekly vaccinations and format for forecast, separating incrementals and cumulative (lagged) vaccinations
3. Run regression analysis to estimate model coefficients; calculate Bass parameters p and q (assume m)
4. Forecast using p, q, m, and cumulative (lagged) vaccinations
5. Plot forecast and output weekly forecast table 
