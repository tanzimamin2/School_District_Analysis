# School District Analysis
This report goes into details about Thomas High School specifically about some discrepancies when it comes to _reading and math grades_.

## Overview of Election audit
The purpose of this report is-
* Replacing ninth-grade reading and math scores
* Generating a new **School District Analysis report** using the new corrected dataset

### Purpose
The main purpose of this report is to analyze the election data and answer the questions mentioned above. This will help the Election Board to determine the winner as well as gathering important statistics about the election.

## Election-Audit Results
Lets take a closer look at the results:-
* _How many votes were cast in this congressional election?_

![image](https://user-images.githubusercontent.com/93144225/142713458-19c89e27-e652-4709-9dbd-af8ef0dfacab.png)

* _Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct._

![image](https://user-images.githubusercontent.com/93144225/142713492-21483446-fac2-40d5-bec7-79a735176825.png)

* _Which county had the largest number of votes?_

![image](https://user-images.githubusercontent.com/93144225/142713509-b3d57aa3-fc1f-471b-98c9-df6e8449ff93.png)

* _Provide a breakdown of the number of votes and the percentage of the total votes each candidate received._

![image](https://user-images.githubusercontent.com/93144225/142713538-2c991d01-cad4-4da0-9b6b-2a3369d0ee63.png)

* _Which candidate won the election, what was their vote count, and what was their percentage of the total votes?_

![image](https://user-images.githubusercontent.com/93144225/142713555-fe11722f-11b9-42f6-9fdc-d5638bf113d4.png)

## Election-Audit Summary
In conclusion, using our Python script is a very easy and efficient way to analyze large datasets and extract the required information.

Manually counting ballots is time consuming as well as labour intensive and there is always a chance for human error. Whereas our Python script can do the same job in a very convinient, accurate and fast manner. This inturn will save money for the Election Board.

With little modifications our script can be used for any elections. Here are two examples:-
* Python is a versatile language and can extract data from numerous file types other then CSV. Modify this line to change the file type. As a result, we can use other types of datasets for any other elections. 

```
# Add our dependencies.
import csv
```

```
# Read the csv and convert it into a list of dictionaries
with open(file_to_load) as election_data:
    reader = csv.reader(election_data)
```

* Our script can easily pull data from any directories of the PC and can output the desired results in any output folders. Modify the following line to change the input dataset and output folders.

```
# Add a variable to load a file from a path.
file_to_load = os.path.join("Resources", "election_results.csv")
# Add a variable to save the file to a path.
file_to_save = os.path.join("analysis", "election_results.txt")
```

* _**Links**_
  * Visit this [link](https://github.com/tanzimamin2/Election_Analysis) for the Python script and other resources.
   
