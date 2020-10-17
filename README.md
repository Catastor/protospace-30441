**ProtoSpace ER**

**users table**
|   column   |  type  | options |
|------------|--------|---------|
|email       |string  |NOT NULL |
|password    |string  |NOT NULL |
|name        |string  |NOT NULL |
|profile     |text    |NOT NULL |
|occupation  |text    |NOT NULL |
|position    |text    |NOT NULL |



**prototypes table**
|   title   |    type    |  option  |
|-----------|------------|----------|
|title      |string      |NOT NULL  |
|catch_copy |text        |NOT NULL  |
|concept    |text        |NOT NULL  |
|image      |            |          |
|user       |references  |          |
**※imageはActiveStorageで実装**



**comments table**
|   title   |    type    |  option  |
|-----------|------------|----------|
|text       |text        |NOT NULL  |
|user       |references  |          |
|prototype  |references  |          |