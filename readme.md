#### Used #####
1. Liquibase 3.8.1 version
2. Mysql docker image
3. Maven tool 

##### Setup #####
1. Run the mysql Docker image

`docker run --name mysql -e MYSQL_ROOT_PASSWORD=<password> -p 3306:3306 -d mysql`

2. `mvn clean install`

3. `mvn resources:resources liquibase:update -Pproduction`

4. For update SQL files

`mvn resources:resources liquibase:updateSQL  -Pdevelopment`

