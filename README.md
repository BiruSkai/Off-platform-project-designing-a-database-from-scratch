# Off-platform-project-designing-a-database-from-scratch 
###### _from codeacademy_
--------------------------
To start this project, it is assumed that the writer is familiar with the following components:
- Tables, columns, data type
- Primary Keys
- Foreign Keys
    - Various types of relationships (one to one, one to many, many to many)

It is recommended to do some research by interviewing someone about a foreign subject which can be related to this project. However, the writter decided to choose a general subject topic on his own experience for this project. 

### Part 1- Brainstorming and Establishing the Diagram
The writter choosed 'Highschool' system. It consists of six entities (the diagram (pdf) can be found in the repository):
1. schools
2. schools_classes_id
3. schools_classes_teachers
4. students
5. teacher_position
6. teachers

The connection between the tables are as follow:
- __one to one__: teachers and teacher_position
- __one to many__: schools and schools_classes_id, students and schools_classes_id, schools_classes_id and schools_classes_teachers
- __many to many__: teachers and schools_classes_teachers

The diagram is created uitlizing an online tool dbdiagram.io .

_Primary key_ on each table is marked with key symbol, while _foreign key_ can be seen on the item of the opposite table to which the table of the primary key is connected. The table having _two primary key with no foreign key_ is schools_classes_teachers. 

### Part 2-- Diagram into A Database Schema
The diagram from dbdiagram.io was exported to PostgreSQL server using Postbird.  Prior to import it in Postbird, several steps are necessary. The detail steps: https://discuss.codecademy.com/t/postgresql-postbird-authentication-method-10-not-supported/557142/6.


### Part 3 -- Add Data To Tables
The writter utilized microsoft excel to add the the majority of the data as this method is efficient. Once completed, the data was transformed to cvs which can be imported by PostgreSql (PgAdmin 4).

### Part 4 -- Test and Edit The Schema 
 Tests were run to examine the ERD (Entities Relationship Diagram) using query tool. Some potential errors have been resolved.  
 
 
