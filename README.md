1. Download the zip file from "https://github.com/Crysicle/BoardGameShopper/tree/main" -> <> Code -> Download ZIP
2. Extract BoardGameShopper
3. Open BoardGameShopper via Intellij:
  File -> Open -> Navigate to BoardGameShopper folder -> click on folder without opening it -> ok.
4. Make sure MariaDB is installed on pc. <br />
  DB and it's tables should auto generate on application start
5. Make sure password and username to access MariaDB are "root" and "root".
  Or go into "hibernate.cfg.xml" file in the BoardGameShopper and change username and password by changing the value assigned to "connection.username" and "connection.password" fields.
6. If running program for the first time: make sure "setupStartingData" in "Main" class is set to true.<br />
  Launching program with "setupStartingData=true" will make the program scrape data from BoardGameGeek and save it to DB.<br />
  On other runs set it to false, otherwise it will continue to rescrape board games each time program is run.
7. Once program is running, go to page "http://localhost:8080/home" you will be redirected to a login page.<br />
  Valid credentials are:<br />
    for ROLE_USER: Username: user, Password: user<br />
    for ROLE_ADMIN: Username: admin, Password: admin<br />
8. Users wont be able to see the search table for board games, admins will.
9. To search for board games via mechanics / category, click on the buttons with said mechanic or category and click "SEARCH" button.
