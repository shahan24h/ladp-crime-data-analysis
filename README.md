# ladp-crime-data-analysis
A lightweight R-based pipeline to clean, sample, and visualize Los Angeles crime data (2020–present).

Los Angeles Police Department (LAPD) Crime Data Analysis
A lightweight R-based pipeline to clean, sample, and visualize Los Angeles crime data (2020–present).
Features
•	Efficient import and cleaning of large CSV datasets
•	Handling of missing values with imputation and filtering
•	Z-score normalization of numeric fields
•	Random sampling for rapid prototyping
•	Age-group analysis and demographic visualizations
•	Cross-tabulation of incidents by age group and location
Requirements
•	R (>= 4.0)
•	R packages: data.table, tidyverse, naniar, lubridate, ggplot2
Install dependencies:
install.packages(c(
  "data.table", "tidyverse", "naniar", "lubridate", "ggplot2"
))
Usage
1.	Clone this repository:
 	
git clone https://github.com/yourusername/LA-crime-analysis.git cd LA-crime-analysis
2. **Place** the raw data file `Crime_Data_from_2020_to_Present.csv` in the `data/` folder.
3. **Run** the cleaning script:
   ```r
source("scripts/clean_crime_data.R")
4.	Generate a sample dataset:
 	
source(“scripts/sample_data.R”)
5. **Knit** the R Markdown report:
   ```bash
Rscript -e "rmarkdown::render('LA_data.Rmd')"
Project Structure
LA-crime-analysis/
├── data/
│   └── Crime_Data_from_2020_to_Present.csv
├── scripts/
│   ├── clean_crime_data.R      # data cleaning pipeline
│   └── sample_data.R           # random sampling script
├── outputs/
│   ├── LA_cleaned_data.csv     # cleaned CSV output
│   ├── LA_crime_5K.csv         # sampled CSV output for 5k
│   └── plots/
│       └── age_group_by_area.png
├── LA_data.Rmd                # analysis report
└── README.txt                 # this file
Contributing
Contributions are welcome! Please open an issue or submit a pull request for changes.
License
This project is licensed under the MIT License.
Access & Use Information
Public: This dataset is intended for public access and use.
Non-Federal: This data set is covered by different Terms of Use than Data.gov. License: See this page for license information.
 
Contact
Shahan – shahan24h@gmail.com
