# Seattle Cars in Bike Lanes

This data curation protocol was created by Sena Crow and Leslie Harka for LIS 545: Data Curation I, taken winter term 2023 for the University of Washington iSchool's MLIS program. It contains data obtained from Sanders Lauture's volunteer data collection project, "Seattle Cars in Bike Lanes." The purpose of the project is to collect public data that helps raise awareness of cars obstructing bike lanes in the City of Seattle. A completely crowdsourced effort, users submit photos and submission details such as the date and location of the bike lane obstruction. Submissions are made via Twitter, Mastodon, or Lauture's website, https://seattle.carinbikelane.com/. The data span 3 months, roughly January to March 2023. 

The dataset consists of 1 CSV file containing crowdsourced reports of bike lane obstructions. Importantly, while this data is largely accessible to most audiences (it’s available via download from the website), as a new initiative started in August 2022, it is incredibly limited. At present, it only includes nine variables and file exports are non-comprehensive (i.e., they don’t include all user submissions). A recent export only contained 73 entries. In our opinion, until the dataset is more representative–containing both more user submissions and capturing other variables of interest for the cause–reuse of this data is less likely. As such, the goal of this protocol is to outline recommendations for variable collection, standard selections, and normalization practices to facilitate the dataset’s potential for reuse and meaningful analysis. Of particular note is our creation of a more robust data dictionary for this dataset, listed in the README file. It includes standard selections and descriptions for seven newly recommended variables in addition to Lauture's original set of nine. 

This dataset is relevant to bike safety advocates, city planners, city officials, and transportation researchers interested in understanding trends regarding cars obstructing bike lanes in the City of Seattle. Incorporation of more details of bike lane obstructions via the variable set we are recommending would improve both analysis and reuse potential. For example, adding data for bike lane, violation, and obstruction types would help quantify and qualify blocked bike lanes (e.g., scope, type, location, and frequency). Insights gained from this analysis would serve to enhance the comparison of future Seattle Cars in Bike Lanes datasets with other existing evidence of urban bike-lane conflicts, such as the City of Seattle’s number of citations given, violation location, and how this compares to their submissions. It is our hope is that our recommendations will serve to inform not only a potential standard data format that is well-described for this issue but also that by doing so advocates can use it to support lobbying efforts focused on making streets safer for cyclists.

## Naming Conventions

Filename: scibl_export_2023-03-02.csv

Short description: A csv file containing a data export of the “Seattle Cars in Bike Lanes” dataset from https://seattle.carinbikelane.com/. 

Data File Naming Conventions: The .csv file name is composed with the following structure:

1. The string "scibl_" representing "Seattle Cars in Bike Lanes" (the title of the dataset produced by Sanders Lauture) followed by an underline.

2. The string “export_” representing the context by which the file was obtained followed by an underline.

3. The date the data was exported is structured as YYYY-MM-DD (e.g. 2023-03-10).


## Data Dictionary

| **Variable** | **Variable Label** | **Measurement Unit** | **Allowed Values** | **Definition** |
| --- | --- | --- | --- | --- |
| Existing dataset variables |
| --- | --- | --- | --- | --- |
| item_id | item id | string | Example: 13d8a866-603c-45fb-8116-cb4f7c94676e.0 | Unique alphanumeric value for each submission that points to the data file for each entry. The value can include  special characters such as punctuation marks and dashes. |
| tweet_time | tweet time | float | Hour values | Hour value in HH:MM:SS format. |
| tweet_date | tweet date | date | YYYY-MM-DD | Date value in YYYY-MM-DD format. |
| number_of_cars | number of cars | integer | >=0 | The total number of cars obstructing the bicycle lane. |
| date | date | date | YYYY-MM-DD | Date value in YYYY-MM-DD format. |
| time | time | float | Hour values | Hour value in HH:MM:SS format. |
| on_street | on street | string | Street name | Name of street segment in which the bicycle lane is obstructed. |
| cross_street | cross street | string | Street name | The nearest intersecting street or road. |
| latitude | latitude | float | ±90° | Latitude of location in decimal degrees. |
| longitude | longitude | float | ±180° | Longitude of location in decimal degrees. |
| image_urls | image urls | string | URL structure (example: http://subdomain.domain.com:1234/) | Full, active URL for image. |
| Recommended additions |
| --- | --- | --- | --- | --- |
| vehicle_type  | vehicle type | string | Example: company, taxi, private owner, municipal, construction, other (damaged lane, snow, debris, pedestrian)  | The type of vehicle or obstruction observed in the bike lane. | 
| tweet_url | Twitter post URL | string | Example: https://twitter.com/carbikelanesea/status/1634021053747060737 | The URL for the Twitter post. |
| toot_url | Mastodon post URL | string | Example: https://social.ridetrans.it/@carbikelanesea/109996668169444818 | The URL for the Mastodon post. | 
| tag_description | post descriptions and tags | string | Examples: delivery, construction, traffic  | User-submitted tags or short  (1-2 words) descriptions that provide more context to the incident. (Curators might move to a controlled list of tags over time). |
| lane_type | bike lane type | string | Example: protected, buffered, painted, etc. | The type of bike lane the car or obstruction was in. |
| car_status | car status | string | Example: parked, driving | Indicates whether a car is parked or driving in the bike lane. |
| council_district | council district | string | District number 1-7; Example: District 3 | The Seattle Council District where the event occurred.|

## Metadata

Schema used: Project Open Data

| **Attribute** | **Value** |
| --- | --- |
| accessLevel | public |
| accrualPeriodicity | R/P1M |
| fn | Sena Crow; Leslie Harka |
| hasEmail | crows3@uw.edu; lharka@uw.edu | 
| describedBy | https://github.com/lharka/lis545_curation-protocol/blob/main/README.md | 
| description | This dataset contains user-submitted reports of cars in Seattle bike lanes. The intended audience(s) are bike advocacy groups and Seattle Department of Transportation. It was curated by Sena Crow and Leslie Harka for a class at the University of Washington in 2023. |
| accessURL |https://github.com/lharka/lis545_curation-protocol |
| downloadURL | https://raw.githubusercontent.com/lharka/lis545_curation-protocol/main/scibl_export_2023-03-02 (Right-click the page and click “Save as”) |
| format |CSV |
| mediaType | CSV |
| issued | 2023-03-09 |
| keyword | “bicycle”, “seattle”, “infrastructure”, “traffic”, “safety”, “car” |
| landingPage | https://github.com/lharka/lis545_curation-protocol |
| language | en-us |
| modified | 2023-03-09 |
| publisher | Sena Crow; Leslie Harka |
| references | https://github.com/golf1052/SeattleCarsInBikeLanes |
| Rights | These data are freely available to the public for all use and reuse |
| temporal | 2023-01-28/2023-02-25 |
| theme | transportation |
| title | Seattle Cars in Bike Lanes |

## Rights

These data are freely available to the public for all use and reuse

## Contact
Sena Crow
crows3@uw.edu

Leslie Harka
lharka@uw.edu
