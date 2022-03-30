This is a very simple code using which you can have db version maintainance for redshift. 
To run it, just do the following:
- Define flyway.url in flyway.conf which will hold your jdbc url of database.
- Define flyway.user in flyway.conf which will hold your user that has permissions to the database.
- Define flyway.password in flyway.conf which will hold the password for the user.
- Add your schema, you want to work with by defining flyway.schemas in flyway.conf. If you don't define it then the default schema which in case of redshift is public will be used.

After that add your scripts. I have some demo scripts added, where you just need to specify your column names and table names.
Finally, run - mvn flyway:migrate

For more details about flyway read here.