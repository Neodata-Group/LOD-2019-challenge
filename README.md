# LOD-2019-challenge

Sample data for Neodata Lab prize of €2000 to the applicant who develops the most accurate algorithm to process an “approximate SQL-like query answering system” on this real dataset. In order to participate in this contest (or if you have any inquiries about the challenge) please send an email to:  lod2019challenge@neodatagroup.com  specifying your full name and affiliation. We will contact you with instructions for downloading the dataset.

All applicants will be given a link to download a real large encrypted dataset. The dataset is composed of two tables, one USER table with about 60M unique user ids and an ACTION table with a total of about 600M rows. Both tables are given in a tab separated format. The USER table is about 2.2Gb while the ACTION table is about 35Gb.

The applicants are required to develop an algorithm to provide an approximate answer to a “SQL-like GROUP BY” query in a given time-frame (a few seconds). Basically, a query should run for no longer than the given time-frame and should return the best approximations for the specified counters (more details below).

Please find all challenge rules in the following:

- The algorithm has to be written in one of the following programming languages: C, Java, Python, R, Scala, Go (if you want to use a different language please contact us);

- The algorithm will receive as input (1) a "condition" C which applies on the given schema and (2) a "time-out in seconds" T. The algorithm has to terminate within T seconds and should return back the most precise counter of the number of tuples matching C. The condition C is something like a standard SQL WHERE clause which can contain any standard SQL operators (including SUBSTRING). Each contestant can choose his/her own syntax for C as long as all possible standard SQL-WHERE operators can be specified. The condition C can spawn over the two input tables (USER and ACTIONS) which are joinable by the user_id field. 

- The final comparison among all algorithms will take place during the conference. All algorithms will be evaulated on the same PC. The evaulating PC will be a Linux machine with Ubuntu 18.10.

- By **July 31st 2019** all applicants have to submit the following:
  - An executable batch file that installs all libraries and tools necessary to support algorithm execution. Please make sure we do not need to do any special operation other than running the script. In case of errors or missing execution the organizers may decide to discard the applicant participation to the contest.
  - An extended abstract, following the conference printing guidelines, that describes the algorithm and the approach in full details. *This abstract will be published in the conference proceedings*.
  - The complete code.
  - Any other support file(s) necessary to execute the algorithm.
  
- On **July 15th 2019** all applicants will receive a set of queries Q, the same set for everyone. *Those are the queries that will be used at conference time to evaluate all algorithms*. The algorithm that, on average, provides the most accurate answers will win the competition. Please note that the queries Q during the competition will be evaulated against some arbitrary time-outs

