# Desafio de projeto DIO Power BI Processando e Transformando Dados

<p align="left">
  <img src="https://github.com/Tiago-Vitali/Desafio-de-projeto-Power-Bi/blob/main/logo.jpg?raw=true" width="150">
</p>

### This project was done as a bootcamp project challenge to DIO Bootcamp "Python Data Analytics Squad.io". It plans to be an introduction to the Microsoft Power BI tool and how to process and transform data using Power Bi.

### After loading the data into Power BI, the following cleaning and transformation steps were carried out::

  - Removal of columns containing metadata in all tables;
  - In the "department" table, the headers were changed: Dname to Dept_Name, Dnumber to Dept_number, Mgr_ssn to Manager_ssn, Mgr_start_date to Manager_start_Date;
  - In the "dept_locations" table changed the headers: Dnumber to Dept_number, Dlocation to Dept_location; LEFT JOIN was carried out with the "department" table, in the resulting table the Dept_name columns were merged with Dept_location, creating the Dept_name_location column and deleting the old ones.
  - In the "employee" table changed the header: Dno to Dept_number. Changed the data type of the Salary column from decimal number to Fixed decimal number (Currency), Divided the Address column into 3 others (Address_number, Address_city, Address_state), Performed LEFT JOIN with the Dept_number column of the "department" table to add the name of each employee's department. Merged the F_name, Minit and Lname columns into the Full_name column. Performed LEFT JOIN of the "employee" table with the "department" table using the Dept_number column to obtain the name of each employee's manager in a new column.
  - In the "project" table, the header was changed: Pnumber to Project_number, Plocation to Project_location, Dnum to Dept_number;
  - In the "works_on" table changed the header: Pno to Project_number;
  - Created a basic report to illustrate some values.
