# :exclamation:logs-analysis-tool:anger:

#**Database content**
this is a tool to aggregate important data from live database using psycopg2 with PostgreSQL database
##:star2:tables contained:star2:

*###log table:running:
this table record the server logs with each client access also this table contains
  * **path**    contain path of article that the client access [foreign key]
  * **ip**      contain ip address that connects to the server
  * **method**  contain the method connection whether it is GET,POST,....
  * **status**  contain the state of connection between server and client whether it is 200 OK or 404 NOTFOUN ,.....
  * **time**    contain the time of each access 
  * **ID**      contain the id number of each connection [primary key]

*###articles table
this table contain the data of each article that is written by each user, this data is contained in the following columns
  * **author**  contain the id number of each author in the authors table [foreign key]
  * **title**   contain the title of each article
  * **slug**    contain a short slug of each article that describes it's content [primary key]
  * **lead**    describes the heading of the entry of each article
  * **body**    the body of each article
  * **time**    the time when this article is written
  * **ID**      specific for each article

*###authors table
this table contain the data about each author who had written or upload the article, this table has columns
  * **name**    contain the name of each author 
  * **ID**      contain the id of each author [primary key]
  * **BIO**     contain the bio of each author
  
  
