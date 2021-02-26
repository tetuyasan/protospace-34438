
#テーブル設計

## userテーブル

| Column      | Type    | Option    |
| -------     | ------- | --------  |
| email       | string  | not.null  |
| password    | string  | not.null  |
| name        | string  | not.null  |
| profile     | text    | not.null  |
| occupation  | text    | not.null  |
| position    | text    | not.null  |

## prototypesテーブル

| Column    | Type       | Option   |
| -------   | --------   | -------  |
| title     | string     | not.null |
| catch_copy| text       | not.null |
| concept   | references | not.null |
| user      |            |          |

## commentsテーブル

| Column    | Type       | Option   |
| -------   | ---------  | -------  |
| text      | text       | not.null |
| user      | references |          |
| prototype | references |          |

