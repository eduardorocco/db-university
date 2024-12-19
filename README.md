1.
```SQL
SELECT * FROM `students`
WHERE YEAR(`date_of_birth`) = 1990
```

2.
```SQL
SELECT * FROM `courses`
WHERE `cfu` > 10
```

3.
```SQL
SELECT * FROM `students`
WHERE TIMESTAMPDIFF(YEAR,`date_of_birth`, CURDATE()) > 30
```
4.
```SQL
SELECT * FROM `courses`
WHERE `period`= 'I semestre'  AND `year` = '1'
```

5.
```SQL
SELECT * FROM `exams`
WHERE HOUR(`hour`) >= 14 AND `date` = '2020-06-20'
```

6.
```SQL
SELECT * FROM `degrees`
WHERE `level` = 'magistrale'
```

7.
```SQL
SELECT COUNT(*) AS number FROM `departments` 
```

8.
```SQL
SELECT COUNT(id) AS total FROM `teachers` 
WHERE `phone` IS NULL
```

9.
```SQL
INSERT INTO `students` (
`degree_id`,
`name`,
`surname`,
`date_of_birth`,
`fiscal_code`, 
`enrolment_date`,
`registration_number`,
`email`) VALUES (
'10',
'Eduardo',
'Rocco',
'1995-07-10',
'RCCDRD95L10F839F',
'2021-10-10',
'77777',
'eduardo_rocco@hotmail.it')
```

10.
```SQL
UPDATE `teachers` SET `office_number` = '126'
WHERE `id` = '58' AND `name` = 'Pietro' AND `surname` = 'Rizzo' 
```