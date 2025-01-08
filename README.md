## Project Overview

The purpose of this project is to explore the effect of higher- or lower-than-expected economic data releases on 2-year and 10-year U.S. Treasury yields.

## Steps Involved:

- Extract data from the Bloomberg Terminal using the API and import it into Excel.

- Define Nonfarm Payrolls (NFP) Survey Delta as the difference between the actual data release and Bloomberg's survey estimate of Wall Street’s forecast:
  - A positive NFP Survey Delta means the change in NFP was higher than forecasted by Wall Street.
    - This can indicate economic strength or strengthening, potentially causing rates to sell off.
  - A negative NFP Survey Delta means the change in NFP was lower than forecasted by Wall Street.
    - This can indicate economic weakness or weakening, potentially causing rates to rally.
  
- Define Unemployment (UE) Survey Delta as the difference between the actual unemployment data release and Bloomberg's survey estimate:
  - A positive UE Survey Delta means the unemployment rate was higher than forecasted by Wall Street.
    - This can indicate economic weakness or weakening, potentially causing rates to rally.
  - A negative UE Survey Delta means the unemployment rate was lower than forecasted by Wall Street.
    - This can indicate economic strength or strengthening, potentially causing rates to sell off.
- Calculate the 10-Year basis point (bps) Delta as the daily change in the 10-Year U.S. Treasury yield (USGG10YR Index) on the release date.
- Calculate the 2-Year basis point (bps) Delta as the daily change in the 2-Year U.S. Treasury yield (USGG2YR Index) on the release date.

- Load the Excel data into Python for further analysis.
- Use Pandas to manipulate and explore the data.

## Current Findings:

- 10-Year Treasury Yield: Daily yield changes for the sample period are normally distributed.
- 2-Year Treasury Yield: Yield changes on NFP release days tend to be positive with higher-than-expected releases and negative with lower-than-expected releases, aligning with the above outlined relationship.
- 10-Year Treasury Yield: Yield changes on NFP release days tend to show no consistent relationship with higher- or lower-than-expected releases.
