# Seattle Cars in Bike Lanes

Add description of dataset overview/abstract. Data curation protocol submission for LIS 545: Data Curation. Taken at the University of Washington during winter term 2023.

Address how the data have been normalized

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
| tag_description | importing any descriptions and tags | string | Examples: delivery, construction, traffic  | User-submitted tags or short  (1-2 words) descriptions that provide more context to the incident. (Curators might move to a controlled list of tags over time). |
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
| downloadURL | (add github link to zip file url) |
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
