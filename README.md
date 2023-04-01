# DS2002 Project 1
> Pawan Jayakumar, George Cao, Kevin Ma

## Documentation:
### Process
We searched Kaggle for three datasets regarding video game sales. The three datasets were: Video Game Sales by Genre, Video Game Sales (EDA, Preprocessing, Modeling), and THE CONSOLE WARS: PS vs Xbox vs Wii. We decided to use the Video Games Genre dataset for our data originating from a NoSQL database (MongoDB), the Video Game Sales dataset for our data originating from a relational database (MySQL), and THE CONSOLE WARS: PS vs Xbox vs Wii dataset as data originating from a file system in CSV format.

Link to the datasets
* [Video Game Sales by Genre](https://www.kaggle.com/datasets/stetsondone/video-game-sales-by-genre)
* [Video Game Sales (EDA, Preprocessing, Modeling)](https://www.kaggle.com/code/ahmedmaher22/video-game-sales-eda-preprocessing-modeling/input)
* [THE CONSOLE WARS: PS vs Xbox vs Wii](https://www.kaggle.com/code/arthurtok/the-console-wars-ps-vs-xbox-vs-wii/input?select=Video_Games_Sales_as_at_22_Dec_2016.csv)

### Code and Deployment Strategy
The Jupyter notebook will connect to MySQL and create a database entitled "videogamesales." To access the MySQL data, we created an SQL file which will import the entries and had the NoSQL data exported as a JSON file. The file stored in a file system will be read as a CSV file. In our Jupyter notebook, we used the csv, json, and mysql.connector libraries to upload and connect all the datasets originating from different sources into the MySQL program. With all the datasets connected, we conducted SQL queries to ensure that the data was processed correctly. An issue we had was importing the dataset to NoSQL, specifically dealing with duplicate titles since games were available on multiple platforms. To solve this, we added IDs to differentiate the entries.

#### What the SQL queries will display:
* Grouping Genre and total sales
* Sales grouped by region
* Critic and User rating per genre
