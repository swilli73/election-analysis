# election-analysis

## Overview of Election Audit

#### The purpose of this election audit was to use newly acquired Python skills to read a CSV file full of votes from an election and display + analyze them in a palatable format. This is done through both printing the results to the command line, as well as a text file. It essentially took what was a messy list of ballots and displayed the total votes cast, the voter turnout from each county (as well as which county had the largest turnout), and the winning candidate along with her vote count and percentage of the vote received. In summary, it quickly and efficiently analyzed a data set and turned it into readable data.


## Election Audit Results

- How many votes were cast in this congressional election?

369,711 votes were cast in total.

- Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.

![Vote Breakdown](https://i.gyazo.com/98a773e28156d8165d156ab78d65e3c2.png)

- Which county had the largest number of votes?

Denver county had the largest voter turnout with 306,055 votes and 82.8% of the total votes.

- Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.

![Candidate Breakdown](https://i.gyazo.com/a84a4465f433fb00014d60268193e508.png)

- Which candidate won the election, what was their vote count, and what was their percentage of the total votes?

![Election Winner](https://i.gyazo.com/88b4b1551fb970b735ecba12d06c65d8.png)

Diana DeGette was the landslide winner of the election, holding 73.8% of the popular vote with 272,892 total votes.

## Election Audit Summary

#### This script is versatile and powerful enough to be used for other elections, as it is a strong outline in itself. This is prominent in how code was reused and slightly modified from collecting the votes of each county to collecting the votes of each candidate. 

![Code Example 1](https://i.gyazo.com/ac3d6a80f7470877095ae8597477a4fc.png)
![Code Example 2](https://i.gyazo.com/5591d6f25c1a1e6b46f2e52496f3b42f.png)

#### The top code was used for determining the winning candidate, and the bottom code was used for determining the winning county. The simple difference is just using different variables and removing one conditional from the winning county as it wasn't needed to display Denver's vote count and percentage, only the fact that it won. 

![Code Example 3](https://i.gyazo.com/fe892952fbfa49acba1da5dd780a3f0c.png)
![Code Example 4](https://i.gyazo.com/f901add5ee53f98bd995736d342ecb9b.png)

#### These are examples of the code used to output/print the winning candidate (left) and the winning county (right). This shows a visual example of what I demonstrated earlier with using different variables and removing conditionals from the winning county count. 
#### As it wasn't necessary to display Denver's vote count and percentage, I removed those from what is essentially the same output code for the winning candidate, but with "winning_county_summary" and "largest_county" variables instead of "winning_candidate_summary" and "winning_candidate" respectively.

![Code Example 5](https://i.gyazo.com/f38e0d5a8305793298b0fd00a4a6b63f.png)
#### This code can be modified and reused to easily accomodate for more votes, more candidates, more counties, all because the outline is here. In fact, the only thing I can think of that would need to be changed is what column the data is taken out of if a new file that doesn't have the Ballot ID, more data in different columns, or all the data scrambled into different columns. 

![Results2](https://i.gyazo.com/062b61311f9c69d68eef9dc845fe523d.png)

#### To even slightly test the capabilities of the script as a strong outline, I randomly inserted "Mickey Mouse" as a candidate and "Cheeseburger" as a county inside of the original CSV file and ran it. While VERY minimally altering the results of the election, it still shows how the script can accomodate edits to the original ballot data with no changes to the code, whether new candidates and/or counties are added.
