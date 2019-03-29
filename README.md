# LOD-2019-challenge
Sample data for Neodata Lab prize of €2000 to the applicant who develops the most accurate algorithm to process an “approximate SQL-like query answering system” on this real dataset. In order to participate in this contest (or if you have any inquiries about the challenge) please send an email to:  lod2019challenge@neodatagroup.com  specifying your full name and affiliation. We will contact you with instructions.

All applicants will be given a link to download a real large encrypted dataset. The dataset is composed of two tables, one USER table with about 60M unique user ids and an ACTION table with a total of about 600M rows. Both tables are given in a tab separated format. The USER table is about 2.2Gb while the action table is about 35Gb.

The applicants are required to develop an algorithm to provide an approximate answer to a “SQL-like GROUP BY” query in a given time-frame (a few seconds/minutes). Basically, a query should run for no longer thanthe given time-frame and should return the best approximations for the specified counters.

During the conference a new sample of data will be used to test all participating algorithms.

The winner is the algorithm who provides the most accurate answer in the given time-frame.
