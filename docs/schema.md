# Schema Information

## Users
column name | data type | other information
------------|-----------|------------------
id          | integer   |
handle      | string    | username, unique, indexed
school_id   | integer   | foreign_key, indexed
email       | string    | unique, set by invite
password_digest | string| unique, set with BCrypt
session_token| string   | reset every session
account_type| integer   | admin, teacher, student with ability to mix, determines account privileges

## Userlinks (allows associations)
column name | data type | other information
------------|-----------|------------------
id          | integer   |
teacher_id  | integer   | foreign_key, indexed
student_id  | integer   | foreign_key, indexed

## School
column name | data type | other information
------------|-----------|------------------
id          | integer   |
number_admins| integer  | acts as limit

## Class
column name | data type | other information
------------|-----------|------------------
id          | integer   |
teacher_id  | integer   | foreign_key, indexed


## Lesson Templates
column name | data type | other information
------------|-----------|------------------
id          | integer   |
name        | string    | unique
subject_id  | integer   | foreign_key, indexed
lesson_text_url | string    | link to text on main site

## Lesson Templatelinks (allows associations)
column name | data type | other information
------------|-----------|------------------
id          | integer   |
lesson_template_id  | integer   | foreign_key, indexed
school_id   | integer   | foreign_key, indexed

## Lessons
column name | data type | other information
------------|-----------|------------------
id          | integer   |
lesson_template_id | integer  | foreign_key, indexed
student_id  | integer   | foreign_key, indexed
class_id    | integer   | foreign_key, indexed
input       | text      | lyrics from student
locked      | boolean   | only modifiable by teachers or admins

## Comments
column name | data type | other information
------------|-----------|------------------
id          | integer   |
lesson_id   | integer   | foreign_key, indexed
teacher_id  | integer   | foreign_key, indexed (may not be necessary)
content     | text      | actual_comments
line_number | integer   | connection to the lesson input
