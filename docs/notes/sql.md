# SQL
- [SQL](#sql)
  - [setting up](#setting-up)
  - [Create \& Insert \& Delete](#create--insert--delete)
    - [DB](#db)
    - [TABLE](#table)
  - [query](#query)
  - [Reference](#reference)


## setting up
- connect to mysql DB with username & password: `mysql -u <<username>> -p`
- mysql setting up with .sql file: `mysql -u <<username>> -p <<database_name>> < setup.sql`


## Create & Insert & Delete
### DB
```bash
SHOW DATABASES;
CREATE DATABASE <database_name>;
USE <database_name>;
DROP DATABASE <database_name>;
DROP DATABASE IF EXIST <database_name>;
```

### TABLE
```SQL
CREATE TABLE
    Users (
        id int AUTO_INCREMENT PRIMARY KEY,
        username varchar(30) NOT NULL UNIQUE,
        account varchar(30) NOT NULL UNIQUE,
        password varchar(255) NOT NULL,
        info varchar(100),
        create_date datetime NOT NULL DEFAULT CURRENT_TIMESTAMP,
        INDEX (username, account)
    );

DROP TABLE IF EXISTS <<table_name>>;

INSERT INTO
    Users (username, account, password, info)
VALUES
    ('username', '123@email.com', 'password', 'hello world');
```

## query
TBD

## Reference
- [SQL 語法教學](https://www.fooish.com/sql/)
- [w3school SQL Tutorial](https://www.w3schools.com/sql/)