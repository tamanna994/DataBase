## Employee Management
- Create employee table
```dtd
CREATE TABLE EMPLOYEE
(
   EmpCode      INT(4),
   EmpFName     VARCHAR(255),
   EmpLName     VARCHAR(255),
   Job          VARCHAR(255),
   Manager      CHAR(4),
   HireDate     DATE,
   Salary       INT(6),
   Commission   INT(6),
   DEPTCODE     INT(2)
);

```
- Insert data inti table
  INSERT INTO EMPLOYEE  
  VALUES (9369, 'TONY', 'STARK', 'SOFTWARE ENGINEER', 7902, '1980-12-17', 2800,0,20),
  (9499, 'TIM', 'ADOLF', 'SALESMAN', 7698, '1981-02-20', 1600, 300,30),    
  (9566, 'KIM', 'JARVIS', 'MANAGER', 7839, '1981-04-02', 3570,0,20),
  (9654, 'SAM', 'MILES', 'SALESMAN', 7698, '1981-09-28', 1250, 1400, 30),
  (9782, 'KEVIN', 'HILL', 'MANAGER', 7839, '1981-06-09', 2940,0,10),
  (9788, 'CONNIE', 'SMITH', 'ANALYST', 7566, '1982-12-09', 3000,0,20),
  (9839, 'ALFRED', 'KINSLEY', 'PRESIDENT', 7566, '1981-11-17', 5000,0, 10),
  (9844, 'PAUL', 'TIMOTHY', 'SALESMAN', 7698, '1981-09-08', 1500,0,30),
  (9876, 'JOHN', 'ASGHAR', 'SOFTWARE ENGINEER', 7788, '1983-01-12',3100,0,20),
  (9900, 'ROSE', 'SUMMERS', 'TECHNICAL LEAD', 7698, '1981-12-03', 2950,0, 20),
  (9902, 'ANDREW', 'FAULKNER', 'ANAYLYST', 7566, '1981-12-03', 3000,0, 10),
  (9934, 'KAREN', 'MATTHEWS', 'SOFTWARE ENGINEER', 7782, '1982-01-23', 3300,0,20),
  (9591, 'WENDY', 'SHAWN', 'SALESMAN', 7698, '1981-02-22', 500,0,30),
  (9698, 'BELLA', 'SWAN', 'MANAGER', 7839, '1981-05-01', 3420, 0,30),
  (9777, 'MADII', 'HIMBURY', 'ANALYST', 7839, '1981-05-01', 2000, 200, NULL),
  (9860, 'ATHENA', 'WILSON', 'ANALYST', 7839, '1992-06-21', 7000, 100, 50),
  (9861, 'JENNIFER', 'HUETTE', 'ANALYST', 7839, '1996-07-01', 5000, 100, 50);




- Employee tables data view
- Query:
```dtd
SELECT * FROM employee;
```
```SQL
+---------+----------+----------+-------------------+---------+------------+--------+------------+----------+
| EmpCode | EmpFName | EmpLName | Job               | Manager | HireDate   | Salary | Commission | DEPTCODE |
+---------+----------+----------+-------------------+---------+------------+--------+------------+----------+
|    9369 | TONY     | STARK    | SOFTWARE ENGINEER | 7902    | 1980-12-17 |   2800 |          0 |       20 |
|    9499 | TIM      | ADOLF    | SALESMAN          | 7698    | 1981-02-20 |   1600 |        300 |       30 |
|    9566 | KIM      | JARVIS   | MANAGER           | 7839    | 1981-04-02 |   3570 |          0 |       20 |
|    9654 | SAM      | MILES    | SALESMAN          | 7698    | 1981-09-28 |   1250 |       1400 |       30 |
|    9782 | KEVIN    | HILL     | MANAGER           | 7839    | 1981-06-09 |   2940 |          0 |       10 |
|    9788 | CONNIE   | SMITH    | ANALYST           | 7566    | 1982-12-09 |   3000 |          0 |       20 |
|    9839 | ALFRED   | KINSLEY  | PRESIDENT         | 7566    | 1981-11-17 |   5000 |          0 |       10 |
|    9844 | PAUL     | TIMOTHY  | SALESMAN          | 7698    | 1981-09-08 |   1500 |          0 |       30 |
|    9876 | JOHN     | ASGHAR   | SOFTWARE ENGINEER | 7788    | 1983-01-12 |   3100 |          0 |       20 |
|    9900 | ROSE     | SUMMERS  | TECHNICAL LEAD    | 7698    | 1981-12-03 |   2950 |          0 |       20 |
|    9902 | ANDREW   | FAULKNER | ANAYLYST          | 7566    | 1981-12-03 |   3000 |          0 |       10 |
|    9934 | KAREN    | MATTHEWS | SOFTWARE ENGINEER | 7782    | 1982-01-23 |   3300 |          0 |       20 |
|    9591 | WENDY    | SHAWN    | SALESMAN          | 7698    | 1981-02-22 |    500 |          0 |       30 |
|    9698 | BELLA    | SWAN     | MANAGER           | 7839    | 1981-05-01 |   3420 |          0 |       30 |
|    9860 | Juie     | israt    | ANALYST           | 7839    | 1992-06-21 |   5000 |        100 |       50 |
|    9861 | JENNIFER | HUETTE   | ANALYST           | 7839    | 1996-07-01 |   5000 |        100 |       50 |
|    9862 | Noshi    | Tamanna  | Student           | 7840    | 1999-12-01 |   3000 |          0 |       10 |
+---------+----------+----------+-------------------+---------+------------+--------+------------+----------+

```

- Between Query:
```dtd
 SELECT * FROM employee WHERE EmpCode BETWEEN 9499 AND 9535;
```
```SQL
+---------+----------+----------+----------+---------+------------+--------+------------+----------+
| EmpCode | EmpFName | EmpLName | Job      | Manager | HireDate   | Salary | Commission | DEPTCODE |
+---------+----------+----------+----------+---------+------------+--------+------------+----------+
|    9499 | TIM      | ADOLF    | SALESMAN | 7698    | 1981-02-20 |   1600 |        300 |       30 |
+---------+----------+----------+----------+---------+------------+--------+------------+----------+
```