# US President election Prediction 
Step 1) We got past Presidential ELction for all 50 States from 1976 to 2012.Last 10 Elections can give us the insights of the trend.The Data can be collected from the US Political Data.

Create Table dem(poll STRING, from_date STRING, to_date STRING, Moe STRING, Clinton

STRING, Sanders STRING, OMalley STRING, Spread STRING, Difference STRING)

ROW FORMAT DELIMITED FIELDS TERMINATED BY ','

STORED AS TEXTFILE LOCATION

'wasb://clusterpresident@cis528president.blob.core.windows.net/PollData_Dem/';

===========

Create Table GOP(poll STRING, from_date STRING, to_date STRING, Trump STRING,

Carson STRING, Rubio STRING, Cruz STRING, Bush STRING, Christie STRING, Fiorina

STRING, Huckabee STRING, Kasich STRING, Paul STRING, Graham STRING, Pataki

STRING, Santorum STRING, Difference STRING)

ROW FORMAT DELIMITED FIELDS TERMINATED BY ','

STORED AS TEXTFILE LOCATION

'wasb://clusterpresident@cis528president.blob.core.windows.net/PollStatistics_Republicans/';

===========

Create Table Age_Fav(age STRING, Clinton STRING, Sanders STRING, Carson STRING, Trump

STRING, Rubio STRING, Cruz STRING, Bush STRING, Christie STRING, Fiorina STRING,

Huckabee STRING, Kasich STRING)

ROW FORMAT DELIMITED FIELDS TERMINATED BY ','

STORED AS TEXTFILE LOCATION

'wasb://clusterpresident@cis528president.blob.core.windows.net/Age_Favourability/';

===========

Create Table Age_Unfav(ageUnf STRING, Clinton STRING, Sanders STRING, Carson STRING,

Trump STRING, Rubio STRING, Cruz STRING, Bush STRING, Christie STRING, Fiorina STRING,

Huckabee STRING, Kasich STRING)

ROW FORMAT DELIMITED FIELDS TERMINATED BY ','

STORED AS TEXTFILE LOCATION

'wasb://clusterpresident@cis528president.blob.core.windows.net/Age_Unfavourable/';

===========

Create Table Ethnicity_fav(ethfav STRING,Clinton STRING, Sanders STRING, Carson STRING,

Trump STRING, Rubio STRING, Cruz STRING)

ROW FORMAT DELIMITED FIELDS TERMINATED BY ','

STORED AS TEXTFILE LOCATION

'wasb://clusterpresident@cis528president.blob.core.windows.net/Ethinicity_Favourability/';

===========

Create Table Ethnicity_Unfav(ethUnfav STRING,Clinton STRING, Sanders STRING, Carson

STRING, Trump STRING, Rubio STRING, Cruz STRING)

ROW FORMAT DELIMITED FIELDS TERMINATED BY ','

STORED AS TEXTFILE LOCATION

'wasb://clusterpresident@cis528president.blob.core.windows.net/Ethinicity_UnFavourability/';

===========

Create Table past_data(State STRING, total STRING, year_1976 STRING, year_1980 STRING,

year_1984 STRING, year_1988 STRING, year_1992 STRING, year_1996 STRING, year_2000

STRING, year_2004 STRING, year_2008 STRING, year_2012 STRING)

ROW FORMAT DELIMITED FIELDS TERMINATED BY ','

STORED AS TEXTFILE LOCATION

'wasb://clusterpresident@cis528president.blob.core.windows.net/Past_Data/';
