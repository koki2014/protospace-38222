


## users テーブル

| Column             | Type   | Options     |
| ------------------ | ------ | ----------- |
| email              | string | null: false |
| encrypted          | string | null: false |
| name               | string | null: false |
| profile            | text   | null: false |
| occupation         | text   | null: false |
| position           | text   | null: false |


## prototypes テーブル

| Column             | Type      | Options                        |
| ------------------ | --------- | ------------------------------ |
| title              | string    | null: false                    |
| catch_copy         | text      | null: false                    |
| concept            | text      | null: false                    |
| user               | reference | null: false, foreign_key: true |


## comments テーブル

| Column             | Type      | Options                        |
| ------------------ | --------- | ------------------------------ |
| content            | text      | null: false                    |
| protetype          | reference | null: false, foreign_key: true |
| user               | reference | null: false, foreign_key: true |

