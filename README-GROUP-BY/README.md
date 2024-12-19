1.
```SQL
SELECT COUNT(*) FROM `students` GROUP BY YEAR(`enrolment_date`)
```

2.
```SQL
SELECT COUNT(*) FROM `teachers` GROUP BY `office_address`
```

3.
```SQL
SELECT AVG(`vote`) FROM `exam_student` GROUP BY `exam_id`
```

4.
```SQL
SELECT COUNT(*) FROM `degrees` GROUP BY `department_id`
```