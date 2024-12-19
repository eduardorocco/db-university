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

