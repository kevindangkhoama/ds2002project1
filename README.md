# DS2002 Project 1
> Pawan Jayakumar, George Cao, Kevin Ma

## Documentation:

### Process
We searched Kaggle for three datasets regarding videogame sales. The three datasets were [Video Game Sales by Genre](https://www.kaggle.com/datasets/stetsondone/video-game-sales-by-genre), [Video Game Sales (EDA , Preprocessing , Modeling)
](https://www.kaggle.com/code/ahmedmaher22/video-game-sales-eda-preprocessing-modeling/notebook), and [THE CONSOLE WARS: PS vs Xbox vs Wii](https://www.kaggle.com/code/arthurtok/the-console-wars-ps-vs-xbox-vs-wii/input?select=Video_Games_Sales_as_at_22_Dec_2016.csv). We decide to use the Video Games Genre dataset for our data originating from a NoSql database (MongoDB), the Video Game Sales dataset for our data originating from a relational database (MySQL), and THE CONSOLE WARS: PS vs Xbox vs Wii dataset as data originating from a file system in a csv format.    

### Code and Deployment Strategy
The jupyter notebook will connect to MySQL and create a database entitled "videogamesales." There we import the three datasets from the three different sources. To access the MySQL data, we created a sql file which will import the entries and had the NoSQL data exported as a JSON file. In our jupyter notebook we used the csv, json, and mysql.connector libraries to connected all the datasets originating from different sources. With all the datasets connected, we conduct sql queries to ensure that the data was processed correctly. An issue we had was importing the dataset to NoSQL, speficially dealing with duplicate titles since games were available in multiple platforms. To solve this, we added IDs to differentiate the entries.

#### What the SQL queries will display:
* Grouping Genre and total sales
* Sales grouped by region
* Count of videogames by genre
