# README

## studentsテーブル

|Column   |Type   |Options    |
|---------|-------|-----------|
|student_name |string |null: false|
|grade |integer |null: false|

### Association
- has_many :coaches 
- has_many :books


## coachesテーブル

|Column   |Type   |Options    |
|---------|-------|-----------|
|coach_name |string |null: false|

### Association
- has_many :students 
- has_many :books


## booksテーブル

|Column   |Type   |Options    |
|---------|-------|-----------|
|title |text |null: false|
|subject |string |null: false|
|start_status |text |null: false|
|finish_status |text |null: false|
|description |text |null: false|
|how_to_use |text |null: false|

### Association
- has_many :coaches 
- has_many :students