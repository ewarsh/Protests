# Background
### Mixed Martial Arts is a very new sport. Data is not being utilized nearly as much as older sports such as Footbal and basketball. This project is the first step in doing this.

# Data
## The ufc_wins database contains a list of winners and losers from all UFC fights from 1993-2019. Each line item contains fighter information as well as landed and attempted for the below types of damage.
### Takedowns
### Ground
### Head
### Significant strikes
### Total Strikes
### Distance
### Body
### Clinch
### Leg

# Data Cleaning
### All landed shots were winsorized to remove outliers.

# Data Exploration/ Feature Selection
### Using the .corr() method, it was determined that takedowns are have the correlation to winning the fight with 7.1%

# Models
## Models used
### K-Nearest Neighbor
### Random Forest
### Support Vector


## Supervised models best results:  K-Nearest Neighbor, K=45
## Accuracy: 	53.5%,	Precision: 	54.1%
### Model had highest accuracy and Precision. Precision is more important than recall because we are only predicting wins.


## Conlcusion
### None of the models created performed very well and it is just as reliable to use the graphical representation to predict that fighters land about 50% of their attempted takedowns. This project is a first pass at a process that can be used more effectively in more specific situations. For example, a fighter knows who their a opponent is months before the event so a data scientist can use this same methodology to look at the primary features that would contribute to beating that opponent. The coach can then structure training camp around the data.
