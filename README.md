1. Extract BoardGameShopper
2. Open BoardGameShopper via Intellij:
  File -> Open -> Navigate to BoardGameShopper folder -> click on folder without opening it -> ok.
3. Make sure MariaDB is installed on pc.
4. Make sure password and username to access MariaDB are "root" and "root".
  Or Go into "hibernate.cfg.xml" file in the BoardGameShopper and change username and password to desired:
        "<property name="connection.username">root</property>"
        "<property name="connection.password">root</property>"
        
5. If running program for the first time: make sure "setupStartingData" in "Main" class is set to true.
  On other runs set it to false, otherwise it will continue to rescrape board games.

6. Once program is running, go to page "http://localhost:8080/home" you will be redirected to a login page.
  Valid credentials are:
    for ROLE_USER: Username: user, Password: user
    for ROLE_ADMIN: Username: admin, Password: admin
7. Users wont be able to see the search table for board games, admins will.

8. To search for board games via mechanics / category, click on the buttons with said mechanic or category and click "SEARCH" button.


