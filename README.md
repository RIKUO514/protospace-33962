
# テーブル設計

## usersテーブル

| Column   | Type   | Options     |
| -------- | ------ | ----------- |
| emall    | string |   NOT NULL  |
| password | string |   NOT NULL  |
|   name   | string |   NOT NULL  |
| profile  |  text  |   NOT NULL  |
|occupation|  text  |   NOT NULL  |
| position |  text  |   NOT NULL  |

### Association

## prototypesテーブル

| Column   | Type     | Options     |
| -------- | -------- | ----------- |
|  title   | string   |   NOT NULL  |
|catch_copy|  text    |   NOT NULL  |
|concept   |  text    |   NOT NULL  |
|   user   |references|             |

### Association

## commentsテーブル

| Column   | Type     | Options     |
| -------- | -------- | ----------- |
|   text   | string   |   NOT NULL  |
|   user   |references|             |
|prototype |references|             |


