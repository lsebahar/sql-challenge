{\rtf1\ansi\ansicpg1252\cocoartf1671\cocoasubrtf600
{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\margl1440\margr1440\vieww10800\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 \'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\
-- Data Engineering\
\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\
\
CREATE TABLE departments (\
  dept_no VARCHAR(30) PRIMARY KEY NOT NULL,\
  dept_name VARCHAR(30) NOT NULL\
);\
\
CREATE TABLE employees (\
  emp_no Integer PRIMARY KEY NOT NULL,\
  birth_date DATE NOT NULL,\
  first_name VARCHAR(30) NOT NULL,\
  last_name VARCHAR(30) NOT NULL,\
  gender VARCHAR(30) NOT NULL,\
  hire_date DATE NOT NULL\
);\
\
CREATE TABLE dept_emp (\
  emp_no Integer NOT NULL,\
  dept_no VARCHAR(30) NOT NULL,\
  from_date DATE NOT NULL,\
  to_date DATE NOT NULL,\
  FOREIGN KEY (dept_no) REFERENCES departments(dept_no),\
  FOREIGN KEY (emp_no) REFERENCES employees(emp_no)\
\pard\pardeftab720\sl340\partightenfactor0
\cf0   PRIMARY KEY (emp_no,dept_no)\
);\
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0
\cf0 \
CREATE TABLE dept_manager (\
  dept_no VARCHAR(30) NOT NULL,\
  emp_no Integer NOT NULL,\
  from_date DATE NOT NULL,\
  to_date DATE NOT NULL,\
  FOREIGN KEY (dept_no) REFERENCES departments(dept_no),\
  FOREIGN KEY (emp_no) REFERENCES employees(emp_no)\
);\
\
\
CREATE TABLE salaries (\
  emp_no Integer NOT NULL,\
  salary Money NOT NULL,\
  from_date DATE NOT NULL,\
  to_date DATE NOT NULL,\
  FOREIGN KEY (emp_no) REFERENCES employees(emp_no)\
  Primary key (emp_no, from_date)	\
);\
\
CREATE TABLE titles (\
  emp_no Integer NOT NULL,\
  title VARCHAR(30) NOT NULL,\
  from_date DATE NOT NULL,\
  to_date DATE NOT NULL,\
  FOREIGN KEY (emp_no) REFERENCES employees(emp_no)\
  Primary Key (emp_no,title,from_date)\
);\
\
--validate imports\
\
select * \
from departments;\
\
select * \
from employees;\
\
select * \
from dept_emp;\
\
select *\
from dept_manager;\
\
select *\
from salaries;\
\
select *\
from titles;\
\
\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\
--Data Analysis\
\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\'97\
\
-- 1) List the following details of each employee: employee number, last name, first name, gender, and salary.\
\
select e.emp_no, e.last_name, e.first_name, e.gender, s.salary\
from employees e\
left join salaries s\
on s.emp_no = e.emp_no;\
\
-- 2) List employees who were hired in 1986. (does this mean current? I assume no.)\
\
select * \
from employees\
where hire_date between '1986-01-01' and '1986-12-31';\
\
-- 3) List the manager of each department with the following information: \
-- department number, department name, the manager's employee number, \
-- last name, first name, and start and end employment dates.\
\
select d.dept_no, d.dept_name, dm.emp_no, e.last_name, e.first_name, dm.from_date as start_date, dm.to_date as end_date\
from departments d\
join dept_manager dm on d.dept_no = dm.dept_no\
join employees e on e.emp_no = dm.emp_no;\
\
-- 4) List the department of each employee with the following information: employee number, last name, first name, and department name.\
\
select de.emp_no, e.last_name, e.first_name, d.dept_name\
from dept_emp de\
join employees e on e.emp_no = de.emp_no\
join departments d on d.dept_no = de.dept_no;\
\
-- 5) List all employees whose first name is "Hercules" and last names begin with "B."\
\
select * \
from employees\
where first_name = 'Hercules'\
and last_name like 'B%';\
\
-- 6) List all employees in the Sales department, including their \
-- employee number, last name, first name, and department name.\
\
select de.emp_no, e.last_name, e.first_name, d.dept_name\
from dept_emp de\
join employees e on e.emp_no = de.emp_no\
join departments d on d.dept_no = de.dept_no\
where dept_name = 'Sales'; \
\
-- 7) List all employees in the Sales and Development departments, \
-- including their employee number, last name, first name, and department name.\
\
select de.emp_no, e.last_name, e.first_name, d.dept_name\
from dept_emp de\
join employees e on e.emp_no = de.emp_no\
join departments d on d.dept_no = de.dept_no\
where dept_name = 'Sales'\
or dept_name = 'Development';\
\
-- 8) In descending order, list the frequency count of\
-- employee last names, i.e., how many employees share each last name.\
\
select last_name, count(last_name) as "count"\
from employees\
group by last_name\
order by count desc;\
\
}