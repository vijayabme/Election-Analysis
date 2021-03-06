# Election-Analysis

## Project Overview
A Colorado Board of Election employee Tom has given us the following tasks to complete the election audit of a recent local congressional election.

1. Calculate the total number of votes cast
2. Get a complete list of candidates who received votes
3. Calculate the total number of votes each candidate received
4. Calculate the percentage of votes each candidate won
5. Determine the winner of the election based on the popular vote

## Resources
- Data Source: election_results.csv
- Software: Python 3.7
- VS Code: 1.48.0

## Summary
The analysis of the election show that:
- There were 369,711 total votes cast in the election
- The candidates were :
    - Charles Casper Stockham
    - Diana DeGette
    - Raymon Anthony Doane
- The chandidate results were:
    - Charles Casper Stockham recevived 23% of the vote and 85,213 number of votes
    - Diana DeGette received 73.8% of the vote and 272,892 number of votes
    - Raymon Anthony Doane 3.1% of the vote and 11,606 number of votes
- The winner of the election was Diana DeGette with 73.8% of the vote and 272,892 number of votes 

## Challenge Overview
The election comission has requested additional data to complete the audit. The following tasks need to be performed to finish the audit
1. The voter turnout for each county
2. The percentage of votes from each county out of the total count
3. The county with the highest turnout

## Challenge Summary
The analysis of the county votes show that:
- There were 369,711 total votes cast in the election
- The counties were :
    - Jefferson
    - Denver
    - Arapahoe
- The county results were :
    - Jefferson received 10.5% of the vote and 38,855 number of votes
    - Denver received 82.8% of the vote and 306,055 number of votes
    - Arapahoe recevied 6.7% of the vote and 24,801 number of votes
- The county with the largest turnout was Denver

## Statement to the election Comission
The code can be used for any election. 
- For example by changing the information in the csv file the code can be run for any number of counties and candidates.
- We can also read from a different file by changing the filename election_results.csv in the code line to a different file name in line 9 of the code
    -  file_to_load = os.path.join("Resources", "election_results.csv")
- If the new file has the candidate name and county name in a different column we just need to replace the numbers inside the row with the new column numbers in the following lines of the code
    -  candidate_name = row[2]
    -  county_name = row[1]
- We can also load the data from an excel file. The following code can be added to read from an excel file
    - import pandas as pd
    - file_to_load = os.path.join("Resources", "Election_results.xlsx")
    - xl = pd.ExcelFile(file_to_load)
    - print(xl.sheet_names)
