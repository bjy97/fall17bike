# Compare Biking data and Zev's model
This Database is used to store biking data and prediction data generated from Zev's model.
## Start the virtual machine:
1. Go to google console at https://console.cloud.google.com, choose My First Project
2. Select the instance `hackplayground` by checking the box on the left and then start the engine by clicking start on top of the page.
3. Open a terminal by clicking on the drop down button on the right side of the instance line, select `open in browser window`

If you don't need to run the application but only needs to look at the database itself, you don't have to do the configuration, skip to "Access the database" section
## Configuration: 
1. Type the command 
```
sudo vim ../../etc/postgresql/9.5/main/pg_hba.conf
```
2.Now you have open up the file pg_hba.conf. Scroll down the document until you see '/32'. Replace the string before the '/' by your IP address found at http://ip4.me/ 
  Note: press "i" to switch to insert mode and after you paste the IP address to the appropriate place, press "esc" to quit the insert mode.
  Press ":x" to quit the document and back to terminal

3. Type the command
```
sudo service postgresql restart
```

## Access the database:
1. Type the command
```
sudo -u postgres psql postgres
```
2. Now you are connected to the database and can see all the tables by typing the command
```
\d
```

## Run the application:
1. In your local terminal, type in the command
```
python air.py
```
2. Copy the IP address appearing below your command line one or two seconds later, paste it in your browser. It should be something like 'http://0.0.0.0:8111/'
