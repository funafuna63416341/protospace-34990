## users テーブル

| Column   | Type   | Options     |
| -------- | ------ | ----------- |
| email    | string | not null    |
| password | string | not null    |
| name     |  text  | not null    |
| profile  | text   | not null    |
|occupation| text   | not null    |
| position | text   | not null    |


## comments テーブル

| Column   | Type     | Options     |
| ------   | -------- | ----------- |
| text     | string   | not null    |
| user     |references|             |
|prototype |references|             |


## prototypesテーブル

| Column | Type       |Options     |
| ------ | ---------- |------------|
| title  | string     | not null   |
|catch_copy| text     | not null   |
|  image   | ActiveStorage|        |
|  user    |references|            |
|  concept | text     | not null   |
