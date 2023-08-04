# SQL_student_database

students table
CREATE TABLE students();
ALTER TABLE students ADD COLUMN student_id SERIAL PRIMARY KEY;
ALTER TABLE students ADD COLUMN first_name VARCHAR(50) NOT NULL;

# set the major_id column from the students table as a foreign key that references the major_id column from the majors table.
ALTER TABLE students ADD FOREIGN KEY(major_id) REFERENCES majors(major_id);

ALTER TABLE majors_courses ADD PRIMARY KEY(major_id, course_id);

