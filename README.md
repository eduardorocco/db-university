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