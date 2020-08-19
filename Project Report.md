#Project Report

## Sources
[Birth Rates](https://www.kaggle.com/cdc/nchs-births-and-birth-rates-data)
[Incarceration Rates](https://commons.wikimedia.org/wiki/File:U.S._incarceration_rates_1925_onwards.png)
[Crime Rates](https://www.ucrdatatool.gov/Search/Crime/State/StatebyState.cfm)

## Types of Transformations
* Joining [Unmarried Births](dirty_csv/UnmarriedBirthsbyAgeGroup1940-2015.csv) and [Total Births](dirty_csv/TotalBirthsandFertilityRate1909-2015)
* Cleaning snd Filtering [Property Crimes](dirty_csv/PropertyCrimeRate1960-2014)

## Final Production Database
MongoDB - Non-relational Database

## Steps
* Extract Incarceration Rated from Wikipedia, download Birth Rates and Property Crime Rates
* Calculate Total Births to Unmarried Women as a percent of Total Births, clean Property Crime Rates by dropping empty columns and removing any cells with NaN
* Transpose DataFrame Dictionaries, upload Dictionaries to MongoDB