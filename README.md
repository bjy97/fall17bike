This Database is used to store biking data and prediction data generated from Zev's model.
To Access the database, follow the following steps:
1. Go to google console at https://console.cloud.google.com
2. Select the instance `hackplayground` by checking the box on the left and then start the engine by clicking start on top of the page.
3. Open a terminal by clicking on the drop down button on the right side of the instance line, select `open in browser window`
3. type the command 
```
sudo -u postgres psql postgres
```
5. Now you are connected to the database and can see all the tables by typing the command
```
\d
```
