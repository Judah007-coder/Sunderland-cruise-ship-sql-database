# Sunderland Cruise Excursions Database

<img width="1536" height="1024" alt="Designer (1)" src="https://github.com/user-attachments/assets/5faeda7b-b40b-491c-94f4-629ae1816c82" />

A relational database built in SQL for a fictional cruise company that sells optional port excursions to passengers. Coursework for IY455 Information Systems Analysis and Design, Nottingham Trent International College (June 2026).

## IMPORTANT NOTE IS THAT IT'S A FICTIONAL COMPANY

# The report
[Sunderland_cruise_ship_report.pdf](https://github.com/user-attachments/files/34537018/Sunderland_cruise_ship_report.pdf)


# What's in the report

The full write-up is in Sunderland_Cruise_Database_Report.pdf. It covers:

Normalising a messy booking table into third normal form (seven tables)
The entity relationship diagram (ERD)
The SQL to create, fill (50 rows per table) and query the database
Six queries, with screenshots of their output

The sample data is fictional and was generated with an AI assistant (Claude) from my table definitions. The design, schema and queries are my own work.


To run it, open the file in a SQL client (I used DataGrip) and run them in that order, since later tables depend on earlier ones.

# What I learnt
Normalisation is about deciding what each piece of data really depends on. Writing my assumptions down made my design choices easier to justify.
Orders and excursions are a many-to-many relationship, which is why that link needed a composite primary key.
Foreign keys force an order of operations. Inserting data in the wrong order fails, so the order of the files matters.
Data types matter. I stored prices as whole numbers, so a 93% price increase turned 35 into 68 instead of 67.55. Next time I would use DECIMAL.

# About me

I'm Praise Ndolo, a BSc Cybersecurity student at Nottingham Trent University, looking for a 12-month industrial placement in cyber security or IT. LinkedIn
