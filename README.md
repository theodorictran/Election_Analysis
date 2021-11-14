# Election_Analysis

## Overview

To assist the Colorado Board of Elections, I was tasked with counting votes of the Congressional Election, determining the winning candidate, and generating a report to summarize the results. Once analysis was complete, to generate a report, I wrote a text file containing the election results.

## Election-Audit Results

- How many votes were cast in this congressional election?
  - There were 369,111 votes casted in this congressional election.
- Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.
  - By county: Denver County had 306,055 votes making up 82.8% of total votes, Jefferson County had 38,855 votes making up 10.5% of total votes, and Arapahoe had 24,801 votes making up 6.7% of total votes.
<img width="191" alt="county_votes" src="https://user-images.githubusercontent.com/91519293/141697974-0074be32-9708-41f9-a8b2-5fd7114d424c.png">
- Which county had the largest number of votes?
  - Denver had the largest number of votes with 306,055 votes casted. Denver accounted for 82.8% of all votes casted in this congressional election.
- Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.
  - By candidate: Diana DeGette received 272,892 votes making up 73.8% of total votes, Charles Casper Stockham received 85,213 votes making up 23.0% of total votes, and Raymon Anthony Doane received 11,606 votes making up 3.1% of total votes.
<img width="290" alt="candidate_votes" src="https://user-images.githubusercontent.com/91519293/141698045-45b5fc2c-cb7c-4491-ad82-1502e4a65b7c.png">
- Which candidate won the election, what was their vote count, and what was their percentage of the total votes?
  - Diana DeGette won the election having 272,892 votes which makes 73.8% of all total votes. 
<img width="209" alt="winning_candidate" src="https://user-images.githubusercontent.com/91519293/141698133-fffd8106-8d3b-4d32-a5eb-10833a813109.png">

Below is a total summary of the election:

<img width="295" alt="election_summary" src="https://user-images.githubusercontent.com/91519293/141698206-21568925-cac1-4269-b638-78f6a95dfe3a.png">

## Election-Audit Summary

- Given how the script was written this scipt can be reused to audit other elections. Assuming that other elections ballots are recorded in the same data structure, meaning the file specifically contains three columns with headers as: Ballot ID, County, and Candidate in a csv file then it is simple to audit any election by simply modifying the file path to the desired file.

  - <img width="472" alt="file_path" src="https://user-images.githubusercontent.com/91519293/141698671-0502085a-7c89-4bd0-bdf8-b38f301b2859.png">
- In reality, having identical file structures is not always possible. In our current dataset, our file contains three columns: Ballot ID, County, and Candidate with 0, 1, and 2 as their respective indexes. There are two statements inside the initial for-loop that iterates through specific columns to either grab county name or candidate name. If a future election contained additional columns and in different orders, then modifying statement to get the candidate name or county name by changing the accompanying index would be performed.
  - <img width="320" alt="for_loop" src="https://user-images.githubusercontent.com/91519293/141699041-3676b2d2-e28b-406f-bd6a-e72ede18a1b5.png">
