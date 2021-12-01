# Visible infraestructure
#### ***MIID course: ETL and data modeling - University of the Andes***
<p align="justify">
Infraestructura visible is an initiative of University of the Andes whose objective is to collect, analyze and centralize information of different government institutions about the current and future infrastructure of Colombia. [link to the project](https://www.infraestructuravisible.org/).

In this course I was tasked with consultant duties. The organization gave us data related with airports and flights from Colombia and they were hoping to solve a set of analytical requirements. The ones that I aimed to solve are listed next:
</p>

  **1. Visualize the number of passengers tranported in a range of dates within Colombia.**
  
  **2. Visualize the number of empty seats in flights in a range of dates within Colombia.**  
  
  **3.  Analize the relationship between the GDP and the number of flights in the department of Colombia.** 

<p align="justify">
For all the three requirements it was implmented an [ETL process](https://github.com/jglobaton10/Visibleinfrastructure/blob/main/ETL.ipynb) that takes the data from a github repository, process it using pyspark and then load into a SQL server database. 
</p>

## Database ER model. 

<img src="diagrama.jpg"  alt="Avatar" style="width:100%">

This [file](https://github.com/jglobaton10/Visibleinfrastructure/blob/main/database.sql) can be used to create and populate the databse. 



<p align="justify">
For the first two requirements it was implemented the following dashboard. The user can track 4 KPI's: total number of passanger, average number of passenger, total number of empty chairs and average number of empty chairs. Also, the user can analize the number of passenger and empty chairs by airport, time and type of airport.  
</p>

<iframe width="680" height="420" src="https://app.powerbi.com/view?r=eyJrIjoiNTg2NmRjYzEtYWM0NS00NzQzLTliMGMtNDI1NTY1ZDc1ZjBmIiwidCI6IjQ0ODhlODRkLWI3NjMtNDUzOC1hY2EyLWU1ZTEwNGNlNTI0NiIsImMiOjN9&pageName=ReportSection" frameborder="0" allowFullScreen="true"></iframe>

<p align="justify">
This is the dashboard implemented for the third requirement. In this case, it has two KPI's total number of passengers and average GDP. The user can analyze the number of flighs and the average GDP per departmente, as well as the GDP change over time, the number of flights per airline and per airport.  
</p>

<iframe width="680" height="420" src="https://app.powerbi.com/view?r=eyJrIjoiNzM5MzIzYzMtY2E1Yy00MDg3LWI3ODYtMzQ3NDVlNGE5OGRmIiwidCI6IjQ0ODhlODRkLWI3NjMtNDUzOC1hY2EyLWU1ZTEwNGNlNTI0NiIsImMiOjN9&pageName=ReportSection" frameborder="0" allowFullScreen="true"></iframe>
