# Liquibase with maven

##### Prechecks
1. Jdk should installed
2. MySql Database
3. Maven installed

If you using windows refer below links for installing maven and java
https://howtodoinjava.com/maven/how-to-install-maven-on-windows/
https://mkyong.com/maven/how-to-install-maven-in-windows/

### Actuall Senario
i have database mysql and i am trying to install the mysql tables using liquibase

1. Build the code
`mvn clean install`

2. Help 
`mvn liquibase:help`

3. Applies the DatabaseChangeLogs to the database. Useful as part of the build process.
`mvn liquibase:update`

##### More info
1. the database table information are at db/src/main/dbschema
2. DB connection properties at db/src/main/dbschema/liquibase.mysql.properties
