# SQL_student_database

students table<br />
CREATE TABLE students();<br />
ALTER TABLE students ADD COLUMN student_id SERIAL PRIMARY KEY;<br />
ALTER TABLE students ADD COLUMN first_name VARCHAR(50) NOT NULL;<br />

# set the major_id column from the students table as a foreign key that references the major_id column from the majors table.
ALTER TABLE students ADD FOREIGN KEY(major_id) REFERENCES majors(major_id);<br />

ALTER TABLE majors_courses ADD PRIMARY KEY(major_id, course_id);

