1.
```SQL
SELECT * FROM `students` JOIN `degrees` ON `degree_id` = `degrees`.id
WHERE degrees.`name` = 'Corso di Laurea in Economia'
```

2.
```SQL
SELECT * FROM `degrees` JOIN `departments` ON `department_id` = `departments`.id
WHERE departments.`name` = 'Dipartimento di Neuroscienze' AND `level` = 'magistrale'
```

3.
```SQL
SELECT * FROM `courses`  JOIN `course_teacher` ON `courses`.id = `course_teacher`.course_id 
JOIN `teachers` ON `teacher_id` = `teachers`.id
WHERE teachers.`name` = 'Fulvio' AND `surname` = 'Amato'
```
4.
```SQL
SELECT * FROM `students` JOIN `degrees` ON `degrees`.id = `students`.degree_id 
JOIN `departments` ON `department_id` = `departments`.id
ORDER BY students.`surname` asc, students.`name` asc
```