
# Table Design

A brief description of what table look like in project database

## Student Full Details
#### Divided into 2 Parts
- StudentDetails

| id | First Name | Middle Name | LastName | gender | DOB | Phone No | Email | Address | Class | Section | Roll No | Photo |
|--|------------|-------------|----------|--------|-----|----------|-------|---------|-------|---------|---------|-------|
| 1 | Prabin| |Gautam|male|2058-03-09|9846915836|prabeen122@gmail.com|Lamjung|12|A|29|**Download**

- Student Parent Info

| id | student_id | Father Name | Mother Name | Address | State | Phone No | Additional Phone | Email | Photo |
|----|------------|-------------|-------------|---------|-------|----------|------------------|-------|-------|
|1|1|Nabaraj Gautam|Usha Gautam|Duipiple|Gandaki|9827***| | ***@gmail.com | **Download** 

## Teacher Details

| id | First Name | Middle Name | LastName | gender | DOB | Phone No | Email | Address | Photo |
|----|------------|-------------|----------|--------|-----|----------|-------|---------|-------|
|1|Mishan| | Khatri|male|205***|98***|**@gmail.com|Pokhara|**Download**

## Assign Teacher A Subject

| id | teacher_id "OR" teacher_name | class | section | subject |
|----|------------------------------|-------|---------|---------|
|1|1 or Mishan Khatri|12|A|DBMS

## Add Classes

| id | class Name | class Code | class Description |
|----|------------|------------|-------------------|
|1|12|A|Class 12 and Section A

## Add Section

| id | class Name "OR" Class ID | Section Name |
|----|--------------------------|--------------|
|1|Class 12 or ID 1|A|
|2|Class 12 or ID 1|B|

## Add Subjects

| id | subject name | subject code | class | section | description |
|----|--------------|--------------|-------|---------|-------------|
|1|DBMS|DBCX|12|A|Description 

## Create Timetables

| id | Day | Start Time | End Time | Subject | Teacher | Class | Section |
|----|-----|------------|----------|---------|---------|-------|---------|
|1|Sunday|10:05 AM|12:50PM|DBMS|Mishan Khatri|12|A

## Attendance

| id | teacher name  | subject | date       | class | section | student name  | roll no | Attendance |
|----|---------------|---------|------------|-------|---------|---------------|---------|------------|
| 1  | Mishan Khatri | DBMS    | 2022-02-25 | 12    | A       | Prabin Gautam | 29      | Absent     |

## Final Marks

| id | class | section | student       | Roll | Remarks |
|----|-------|---------|---------------|------|---------|
| 1  | 12    | A       | Prabin Gautam | 29   | Passed  |

## Announcements

| id | type      | for     | class | section | title | Created Date | Created BY | Creator Name or Creator ID                                                         |
|----|-----------|---------|-------|---------|-------|--------------|------------|------------------------------------------------------------------------------------|
| 1  | Admission | Teacher |       |         | Hello | 2021-12-05   | Admin      | Prabin Gautam \|\| Id of Prabin Gautam Needed (To show profile picture of Creator) |

## Assignment Given BY teacher_id

| id | teacher  | class | section | subject | title | date due | time due | instruction | created date | file |
|----|----------|-------|---------|---------|-------|----------|----------|-------------|--------------|------|

## Assignment Submitted By Student

| id | assignment id | student name  | student roll | status     | submitted date | submitted time | file | remark    |
|----|---------------|---------------|--------------|------------|----------------|----------------|------|-----------|
| 1  | 2             | Prabin Gautam | 29           | Submitted  | 2022-02-05     | 12:05 AM       | --   | Well done |
| 2  | 2             | Paras Panta   | 28           | Pending    |                |                |      |           |

## Internal Reports

| id | teacher | class | section | subject | student | roll no | marks |
|----|---------|-------|---------|---------|---------|---------|-------|
|1|Mishan Khatri|12|A|DBMS|Prabin Gautam|29|99.9

##Lecture Notes

| id | class | section | subject | teacher       | description           | file         |
|----|-------|---------|---------|---------------|-----------------------|--------------|
| 1  | 12    | A       | DBMS    | Mishan Khatri | Subject Notes of DBMS | **Download** |
