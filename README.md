##### Virat Kohli Cricket Career Analysis Dashboard

An interactive **Power BI dashboard** created to analyse Virat Kohli's ICC cricket career across a 15-year period. The report presents major batting statistics, opponent-wise performance, yearly run trends, and interactive date-based filtering in a clean sports-themed layout.

##### Dashboard Overview

The full dashboard snapshot covers the period from **18 August 2008 to 14 July 2022** and displays the following headline statistics:

|KPI|Value|
|-|-:|
|Matches|516|
|Runs|24K|
|Highest Score|254|
|Batting Average|45.95|

> KPI values change automatically when the date range or another visual is selected.

##### Key Features

* Interactive start-date and end-date slicer
* Dynamic KPI cards for matches, runs, highest score, and average
* Opponent-wise run comparison using a column chart
* Opponent-wise total-match distribution using a doughnut chart
* Year-by-year run analysis using an area chart
* Cross-filtering between charts and KPI cards
* Calendar-based date selection
* Sports-themed dashboard design featuring Virat Kohli

##### Dashboard Visuals

##### 1\. KPI Cards

The dashboard contains four summary cards:

* **Matches:** Total count of matches in the selected period
* **Runs:** Sum of runs scored in the selected period
* **Highest:** Maximum individual score in the selected period
* **Average:** Average runs for the selected period

##### 2\. Runs by Opponent

A column chart compares the total runs scored against major opponents, including:

* Australia
* England
* West Indies
* Sri Lanka
* South Africa

In the complete dashboard view, Australia has the highest run total among the opponents displayed.

##### 3\. Total Matches by Opponent

A doughnut chart displays the opponent-wise contribution to the total-match metric. Selecting an opponent filters the remaining dashboard visuals.

##### 4\. Runs by Year

The area chart shows the yearly run trend throughout the selected career period. The dashboard indicates strong run accumulation during the middle and later years of the career, followed by a noticeable decline after 2019.

##### 5\. Date Range Slicer

The date slicer allows users to:

* Drag the start and end handles
* Enter dates manually
* Select dates using the calendar
* Analyse performance within a specific career period

Changing the date range updates every KPI and chart on the page.

##### Dataset Fields

The Power BI data model visible in the project contains the following fields:

|Field|Description|
|-|-|
|`date`|Match date|
|`ground`|Match venue or ground|
|`index`|Row/index identifier|
|`match`|Match-related field used for counting matches|
|`Match\\\_No`|Match number|
|`opponent`|Opposing team|
|`runs`|Runs scored|
|`total`|Total-match related value used in the opponent distribution|

##### Visual Field Mapping

|Visual|Category / Axis|Value|
|-|-|-|
|Date slicer|`date`|Date range|
|Matches card|-|Count of `match`|
|Runs card|-|Sum of `runs`|
|Highest card|-|Maximum of `runs`|
|Average card|-|Average of `runs`|
|Runs - Opponent|`opponent`|Sum of `runs`|
|Total Matches - Opponent|`opponent`|`total` metric|
|Runs - Year|Year from `date`|Sum of `runs`|

##### Interactivity Demonstrated

The dashboard demonstration shows that users can:

1. Adjust the date slider to analyse different career periods.
2. Use the calendar to select an exact start or end date.
3. Click an opponent bar such as Australia or South Africa.
4. Cross-filter the KPI cards, doughnut chart, and yearly trend chart.
5. Click outside the selected visual to restore the complete dashboard view.

##### Tools Used

* Microsoft Power BI Desktop
* Power BI interactive visuals
* Date slicer and calendar filter
* Card, column, doughnut, and area chart visuals
* Structured cricket performance dataset

##### Project Files

```text
Virat-Kohli-Score-Analysis/
├── README.md
├── Virat Kohli pdf.pdf
├── Virat v 2.mp4
└── Virat-Kohli-Score-Analysis.pbix
```

* [View the dashboard PDF](./Virat%20Kohli%20pdf.pdf)
* [Watch the dashboard demonstration](./Virat%20v%202.mp4)

##### How to Use

1. Download or clone the project repository.
2. Open the `.pbix` file using Microsoft Power BI Desktop.
3. Refresh the data if the original data source is available.
4. Use the date slicer to select a career period.
5. Select chart elements to explore opponent-wise and year-wise performance.
6. Use the PDF for a static dashboard preview and the MP4 file for the interaction demonstration.

##### Dashboard Highlights

* Clean white-and-blue cricket theme
* Large Virat Kohli cut-out integrated into the layout
* Stadium background with low opacity for better readability
* Important statistics visible at a glance
* Simple navigation and interactive analysis suitable for academic presentation

##### Disclaimer

This dashboard is an educational data-visualisation project. It is not officially affiliated with Virat Kohli, the ICC, or any cricket board. Statistics shown in the report depend on the dataset used in the Power BI project.

