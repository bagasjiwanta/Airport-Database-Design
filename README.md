# Airport-Database-Design

An airport database design based on Soekarno-Hatta International Airport in Jakarta. Contains almost all aspects of an airport, such as pilots, tickets, employees, airlines, airplane models, etc.\

## How we built it


## How to use
Since this sql is created and tested using mariadb, you need to have mariadb on your computer to use it.
1. Download the repository, and then go to the root folder 
2. Open up mariadb and create a database called `soetta`
```sql
create database soetta
```
3. import the sql file using this command
```sql
use soetta
\. airport.sql
```
4. To make sure things work, use this example command
```sql
select airline_name from airline where airline_id = 104;
```
make sure you got the similar result (ignore the time)
```
MariaDB [soetta]> select airline_name from airline where airline_id = 104;
+---------------+
| airline_name  |
+---------------+
| THAI LION AIR |
+---------------+
1 row in set (0.072 sec)
```
