
# Goal of the project

- Collect the data of a subset of wikipedia pages with information like number of views and access type , perform few data processing and save the data in json formats. 
- Use the data to perform time series analysis of articles traffic.

# Licences and terms & conditions

Repo licence:

[![MIT License][license-shield]][license-url]

Source data licence:

[CC-BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) 

[GFDL](https://www.gnu.org/copyleft/fdl.html) 

# Souce data

[Pageview API documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews)

[Terms and conditions](https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions)
 
# Output

The notebook is divided into 2 parts:

- Data Acquisition
- Data Analysis

## Data Acquisition
- Pageviews API is used to collect time series data of article traffic from July 2015 to September 2022.
- The data counts the pageviews for a subset of wikipedia pages which are basically [dinosaurs related articles](https://github.com/khirodsahoo93/data-512-homework_1/blob/main/dinosaurs.csv).
- The data is processed ,converted to json format and saved in 3 different json files.
  1. Pageviews count for mobile- dino_monthly_mobile_201507-202209.json
  2. PageViews count for desktop- dino_monthly_desktop_201507-202209.json
  3. Pageviews count for cumulative all-access - dino_monthly_cumulative_201507-202209.json

## Data Analysis

- Intermediate files to generate the visualizations are stored in this [folder](https://github.com/khirodsahoo93/data-512-homework_1/tree/main/csv_data).
- Three different charts were generated and saved in [output](https://github.com/khirodsahoo93/data-512-homework_1/tree/main/charts) folder.
   1. Maximum Average and Minimum Average - The graph contains time series for the articles that have the highest average page requests and the lowest average page  
      requests for desktop access and mobile access. 
   2. Top 10 Peak Page Views - The second graph contains time series for the top 10 article pages by largest (peak) page views over the entire time by access type.
   3. Fewest Months of Data - The third graph displays pages that have the fewest months of available data.

 

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[license-url]:https://github.com/khirodsahoo93/data-512-homework_1/blob/main/LICENSE
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
