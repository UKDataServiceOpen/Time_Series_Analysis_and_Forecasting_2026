![UKDS Logo](./assets/images/UKDS_Logos_Col_Grey_300dpi.png)<br> <br>

# Time Series Analysis and Forecasting

This repo contains the material from the 2026 UKDS workshop named 'An Introduction to Time Series Analysis and Forecasting'. In this repo you will find the slide deck, the code from the RProject as well as the interactive code found below.  

## Interactive Coding Materials

You have **three options** to run the workshop:  

1️⃣ **Run Locally in RStudio** 

Download the files and run them on your computer. Simply follow the instructions in the code_demo.Rmd file. 

2️⃣ **Run Online in Google Colab** 

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/UKDataServiceOpen/Time_Series_Analysis_and_Forecasting_2026/blob/main/code_demo.ipynb)

3️⃣ **Open in Posit Cloud**

[![Open in Posit Cloud](https://img.shields.io/badge/Open%20in-Posit%20Cloud-blue?logo=rstudio)](https://posit.cloud/content/13306443)


## Further Material

Users should feel free to peruse the materials here as well as watch the recordings made during the various workshops on the UK Data Service YouTube channel. https://www.youtube.com/user/UKDataService

* To access learning materials from the wider *Computational Social Science* training series: <a href="https://github.com/UKDataServiceOpen/computational-social-science" target=_blank>[Training Materials]</a>
* To keep up to date with upcoming and past training events: <a href="https://ukdataservice.ac.uk/training-events/" target=_blank>[Events]</a>
* To get in contact with feedback, ideas or to seek assistance: <a href="https://ukdataservice.ac.uk/help.aspx" target=_blank>[Help]</a>

## 📊 Data Sources

1. **Crime Data (Detroit, 2015–2020)**
   Ashby, M. P. J. (2019). Studying Crime and Place with the Crime Open Database. *Research Data Journal for the Humanities and Social Sciences, 4*(1), 65–80. https://doi.org/10.1163/24523666-00401007. Data retrieved [2015-2026] from https://osf.io/zyaqn/

2. **Age of Death of Kings of England**
   Hyndman, R., & Yang, Y. (2018). *tsdl: Time Series Data Library* (v0.1.0). https://pkg.yangzhuoranyang.com/tsdl/. Data retrieved [date] from https://robjhyndman.com/tsdldata/misc/kings.dat. Source listed in the data file: McNeill, *Interactive Data Analysis*.

3. **Monthly Births in New York City, 1946–1959**
   Hyndman, R., & Yang, Y. (2018). *tsdl: Time Series Data Library* (v0.1.0). https://pkg.yangzhuoranyang.com/tsdl/. Data retrieved [date] from http://robjhyndman.com/tsdldata/data/nybirths.dat. Originally collected by Newton.

4. **Monthly Temperatures at Nottingham, 1920–1939 (`nottem`)**
   Anderson, O. D. (1976). *Time Series Analysis and Forecasting: The Box-Jenkins Approach*. Butterworths. Series R. Accessed through the R `datasets` package.

## Data Sources & Licensing

This workshop uses police-recorded crime data from the Crime Open Database (CODE), accessed through the `crimedata` R package, alongside three teaching datasets. No data files are stored in this repository; the code downloads or loads them when it runs. Licensing terms differ by dataset, so check each source before reusing the data.

---

### 1. Crime Open Database (Detroit, 2015–2020)

**Source:** Crime Open Database — [osf.io/zyaqn](https://osf.io/zyaqn/)
**Accessed with:** `crimedata::get_crime_data(cities = "Detroit", years = 2015:2020, type = "core")`
**Licence:** Free to use with acknowledgement of the source.

### 2. Kings and 3. Births

**Source:** Time Series Data Library — [robjhyndman.com/TSDL](https://robjhyndman.com/TSDL/)
**Licence:** 

### 4. nottem

**Source:** R `datasets` package, included with R
**Licence:** 

---

## Software

Ashby, M. (2023). *crimedata: Access Crime Data from the Open Crime Database* (R package version 0.3.5; MIT licence). https://doi.org/10.32614/CRAN.package.crimedata

## Methods Reference

The SARIMA forecasting approach was adapted from:
Ashby, M. P. J. (2020). Initial evidence on the relationship between the coronavirus pandemic and crime in the United States. *Crime Science, 9*, Article 6. https://doi.org/10.1186/s40163-020-00117-6
