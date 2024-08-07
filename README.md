# nosql-challenge
-----------------
> In this challenge, I worked with a json file of restaurant data. The goal was to put the data into a workable db for easy analysis.
> After the data was set into a database, the database was cleaned and updated. Once updated, I ran some analysis and created dataframes for each result.
> > <img src="./img/nosql_img1.png" alt="Dataframe" width="800"/>
### Database and Jupyter Notebook Set Up
-----------------------------------------
- Data imported using the following text: `mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json`
- Listed DB available and collections in the DB
- Displayed one document in the collection
- Assigned the collection into a variable for use.

### Update the Database
-----------------------
- Inserted a new document to the collection using **__insert_one__**
- Update datatypes on columns using **__update_many__** 
- Removed data that is not relevant using **__delete_many__**
- Query data with **.find(query,fields)**
<img src="./img/nosql_img2.png" alt="insert_one" width="800"/>

### Analysis
------------
- Query collections to find establishments with a target hygiene score
- Determined the number of establishments that are overseen by a specific Local Authority
- Searched establishments in a given geographical location by a radius of .01 degree (lat, long)
- Created dataframes for anaylsis results
<img src="./img/nosql_img3.png" alt="'$regex'" width="800"/>
