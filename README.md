# ODA Multilateral sector imputations
This repository showcases how to replicate ONE's multilateral sectors imputations.

## What is the difference between bilateral and multilateral development assistance?

DAC data on donor countries’ ODA measure the outflow of resources and divide it into two categories: bilateral and multilateral. Total ODA figures, for example, include donors’ direct contributions to developing countries plus their contribution to the multilateral system.

Multilateral ODA consists of the contributions provided to multilateral organisations that are not earmarked. By definition, therefore, these contributions are not disaggregated by country or region.

The DAC reports how much donors have contributed to each multilateral agency. It also reports on how much has been spent by most multilateral agencies, by country and sector. As part of its standard set of statistics, the DAC estimates what proportion of each DAC donor country’s contribution to multilateral agencies can be imputed for each developing country or region. This is what is commonly referred to as “imputed multilateral aid”.

Sectoral imputed multilateral aid data is similar to “imputed multilateral aid” but it is further disaggregated in order to estimate how spending by multilateral agencies targeting specific sectors can be imputed to each DAC donor country.


## How are ONE’s sectoral imputed multilateral aid numbers calculated?

ONE’s methodology for calculating sectoral imputed multilateral aid is based on the approach previously used by the OECD. The primary objective of our imputations is to present a more comprehensive picture of bilateral donors’ sectoral spending by including estimates of the sectors that are targeted through their core contributions to the multilateral system.

As the OECD notes elsewhere, any methodology for imputing multilateral flows can only ever be seen as an approximation. Delays in reporting, incomplete data on multilateral outflows, turning grants into loans, and restrictions on pooling mean that multilateral outflows in a given year do not exactly match bilateral donors’ core contributions to the multilateral system.


## Sectoral imputed multilateral aid for a given DAC donor is calculated following three broad steps:

### Step 1
Using data from the Creditor Reporting System, we calculate each multilateral agency's total flows to a given sector as a share of its total spending (core resources only). Whenever possible, sectoral spending is analysed at the ‘CRS agency’ level.

Both ODA and OOF are taken into account at this stage, following previous OECD practice. Similarly, three-year spending data are used to produce the sector spending shares. That means that the shares for year n are produced using spending data for years n, n-1 and n-2.

### Step 2
Using data from the Members Total Use of the Multilateral System database, we calculate the bilateral donor’s core ODA contributions to each multilateral agency (for year n). Where possible, the inflow amounts for each multilateral organisation are calculated at the ‘CRS agency’ level.

### Step 3
For each donor, sectoral imputed multilateral aid figures are calculated by multiplying the contributions made to each multilateral organisation (obtained through step 2) by the sector spending shares for each specific multilateral organisation (obtained through step 1). 


### Example
The World Bank’s International Development Association (IDA) allocated 8.5% of its resources to the Education sector over 2017-2019.
France provided US $444 million to IDA as core resources in 2019.
France’s imputed multilateral aid to the health sector through IDA for 2019 was US$ 37.8 million (8.5% of its US $444 million core contribution to IDA)

To calculate France’s total sectoral imputed multilateral aid, the same calculations are repeated for every multilateral agency, for every sector.


There is a key difference between ONE’s approach and the (discontinued) OECD approach: ONE’s imputations focus on (gross) disbursements rather than commitments. This applies throughout: for multilateral spending shares, for core contributions inflows data, and for the resulting sectoral multilateral imputed aid numbers.


## Data sources
This research uses data from the DAC Creditor Reporting System (CRS) and the Members Total Use of the Multilateral System database. The CRS is a database containing data on aid activities reported by the DAC members. The Members Total Use of the Multilateral System database contains data on core contributions
to the budgets of multilateral agencies. Both databases are maintained by the OECD.


## Using the tool
This project uses `poetry` to manage python dependencies. It requires python>=3.10.

After creating a virtual environment for this project, you can install project dependencies
by running the following command with your terminal at the project root.

You must have `poetry` installed in your environment first.

```bash
poetry install
```