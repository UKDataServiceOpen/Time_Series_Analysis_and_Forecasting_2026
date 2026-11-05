![UK Data Service logo](./assets/images/UKDS_Logos_Col_Grey_300dpi.png)

# Time Series Analysis and Forecasting

This repository contains the materials from the 2026 UK Data Service workshop, *An Introduction to Time Series Analysis and Forecasting*. It includes the slide deck, the R Project code and the interactive notebook linked below.

## Interactive Coding Materials

Choose one of these three ways to follow along. All of them use the same workshop content.

| Option | Best for | What you need |
|---|---|---|
| [**1. RStudio**](#1-run-locally-in-rstudio) | Keeping and reusing the materials | R, RStudio and Git |
| [**2. Google Colab**](#2-run-online-in-google-colab) | Running the code without installing anything | A Google account |
| [**3. Posit Cloud**](#3-run-online-in-posit-cloud) | Using RStudio in your browser | A Posit Cloud account |

### 1. Run locally in RStudio

**Before you start,** install [R](https://cran.r-project.org/), [RStudio](https://posit.co/download/rstudio-desktop/) and [Git](https://git-scm.com/downloads).

**Clone the repository:**

1. In RStudio, go to **File > New Project > Version Control > Git**.
2. Under **Repository URL**, paste:

   ```text
   https://github.com/UKDataServiceOpen/Time_Series_Analysis_and_Forecasting_2026
   ```

3. Under **Create project as subdirectory of**, choose where to save the project.
4. Tick **Open in new session** and click **Create Project**.

**Run the workshop:**

1. In the **Files** pane, open `code_demo.Rmd`.
2. Run the install chunks once to install the required packages.
3. Work through the remaining chunks by clicking the green **Run** arrow at the top right of each one.

**Don't have Git?** On this repository's GitHub page, select **Code > Download ZIP** and unzip the folder. Then open RStudio, go to **File > New Project > Existing Directory**, select the folder and open `code_demo.Rmd`.

### 2. Run online in Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/UKDataServiceOpen/Time_Series_Analysis_and_Forecasting_2026/blob/main/code_demo.ipynb)

1. Click the badge and sign in to your Google account.
2. Run the cells in order from the top. Installing the packages may take a while.
3. To keep your changes, select **File > Save a copy in Drive**.

### 3. Run online in Posit Cloud

[![Open in Posit Cloud](https://img.shields.io/badge/Open%20in-Posit%20Cloud-blue?logo=rstudio)](https://posit.cloud/content/13306443)

1. Click the badge and log in, or create a free account.
2. Open `code_demo.Rmd` in the **Files** pane.
3. Run the chunks in order from the top.

You'll get your own temporary copy of the project, so your changes won't affect anyone else. To keep your work, save a permanent copy to your workspace.

## Further Materials

- **Workshop recordings:** [UK Data Service YouTube channel](https://www.youtube.com/user/UKDataService)
- **Wider training series:** [Computational Social Science materials](https://github.com/UKDataServiceOpen/computational-social-science)
- **Upcoming and past events:** [UK Data Service training and events](https://ukdataservice.ac.uk/training-events/)
- **Feedback, ideas or help:** [Contact the UK Data Service](https://ukdataservice.ac.uk/help.aspx)

## Data Sources and Licensing

This workshop uses police-recorded crime data from the Crime Open Database (CODE), accessed through the `crimedata` R package, alongside three teaching datasets. No data files are stored in this repository; the code downloads or loads them when it runs. Licensing terms differ by dataset, so check each source before reusing the data.

### 1. Crime data: Detroit, 2015–2020

- **Source:** [Crime Open Database](https://osf.io/zyaqn/)
- **Accessed with:** `crimedata::get_crime_data(cities = "Detroit", years = 2015:2020, type = "core")`
- **Licence:** Free to use with acknowledgement of the source.
- **Citation:** Ashby, M. P. J. (2019). Studying Crime and Place with the Crime Open Database. *Research Data Journal for the Humanities and Social Sciences, 4*(1), 65–80. https://doi.org/10.1163/24523666-00401007. Data retrieved [date] from https://osf.io/zyaqn/

### 2. Age of death of the kings of England

- **Source:** [Time Series Data Library](https://robjhyndman.com/TSDL/)
- **Licence:** [To be confirmed]
- **Citation:** Hyndman, R., & Yang, Y. (2018). *tsdl: Time Series Data Library* (v0.1.0). https://pkg.yangzhuoranyang.com/tsdl/. Data retrieved [date] from https://robjhyndman.com/tsdldata/misc/kings.dat. Source listed in the data file: McNeill, *Interactive Data Analysis*.

### 3. Monthly births in New York City, 1946–1959

- **Source:** [Time Series Data Library](https://robjhyndman.com/TSDL/)
- **Licence:** [To be confirmed]
- **Citation:** Hyndman, R., & Yang, Y. (2018). *tsdl: Time Series Data Library* (v0.1.0). https://pkg.yangzhuoranyang.com/tsdl/. Data retrieved [date] from http://robjhyndman.com/tsdldata/data/nybirths.dat. Originally collected by Newton.

### 4. Monthly temperatures at Nottingham, 1920–1939 (`nottem`)

- **Source:** R `datasets` package, included with R
- **Licence:** [To be confirmed]
- **Citation:** Anderson, O. D. (1976). *Time Series Analysis and Forecasting: The Box-Jenkins Approach*. Butterworths. Series R. Accessed through the R `datasets` package.

## Software

Ashby, M. (2023). *crimedata: Access Crime Data from the Open Crime Database* (R package version 0.3.5; MIT licence). https://doi.org/10.32614/CRAN.package.crimedata

## Methods Reference

The SARIMA forecasting approach was adapted from:

Ashby, M. P. J. (2020). Initial evidence on the relationship between the coronavirus pandemic and crime in the United States. *Crime Science, 9*, Article 6. https://doi.org/10.1186/s40163-020-00117-6
