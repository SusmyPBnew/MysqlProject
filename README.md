# MysqlProject
                                                               
    
  ## Library Management System(MySql Project)

  <p>In this project describes about the some sql queries implement to get the data under Library Management System.Library have huge collections of books,so we have to get categorize data using this sql queries</p>

  For writing queries we need to store the data in particular tables,which describes below,

  ## Tables for Storing Library Management Data

<ol>
<li>Branch: This table for storing no of library branches,that including fields like branch_no(<b>primary key</b>), manager_id,branch_address, and contact_no.</li>

<li>Employee: This table for storing employees details working under the these branches,that including fields like employee_id(<b>primary key</b>), name, position, salary, and the branch_no(<b>foreign key</b>).</li>

<li>Books:  This table for storing books details that available in all libraries ,that including fields like ISBN(<b>primary key</b>), title, category, rental price,status(we need to set "yes" or "no", author, and publisher.</li>

<li>Customer: This table for storing customer deatails him/her buy a particular book from any library,that including fields like customer_id(<b>primary key</b>), name, address, and registration date.</li>

<li>IssueStatus: This table for storing issued books by customer details,that including fields like issue_id(<b>primary key</b>), customer_id(<b>foreign key</b>), book name, issue date, and ISBN(<b>foreign key</b>).</li>

<li>ReturnStatus: This table for storing retured books by customer details,that including fields like return_id(<b>primary key</b>), customer_id(<b>foreign key</b>), book name, return date, and ISBN(<b>foreign key</b>).</li>
</ol>


###### *Note : PRIMARY KEY specify above, is a column in a relational database table that's distinctive for each record and A FOREIGN KEY is a field (or collection of fields) in one table, that refers to the PRIMARY KEY in another table.

## Process follows this Project

<ul>
<li>First of all we creating a database using the following command,</li>
          create database Library;
  <li>Then we shows the current databases(not necessary)</li>
          show databases;
  <li>After that we using that newly created DB using below command,</li>
           use Library;
  <li>Then creating new tables(listed above) for storing the data needed for this project</li>
     Syntax: create table TABLENAME(columns1 datatype1,columns2 datatype2,.........);
 <li>Then insert values in that tables,</li>
  Syntax:insert into TABLENAME values(value1,value2,.......);

<li>After that we solve some queries for that different operations that done under library management system</li>
</ul>

## MySql queries for Fetching Particular Information

<ol>
<li> Retrieve the book title, category, and rental price of all available books.</li>
  This results for using select  command and return title, category, and rental price from BOOKS table.
 <li> List the employee names and their respective salaries in descending order of salary.</li>
    This results for using select command and return employee names and their respective salaries that salary in descending order from EMPLOYEE table.
<li> Retrieve the book titles and the corresponding customers who have issued those books.</li>
      This results for using select command and return titles and the corresponding customers by joining CUSTOMER and ISSUE table using join command.
<li> Display the total count of books in each category.</li>
        This results for using select command and return total count of books from BOOKS table using group by command.
<li> Retrieve the employee names and their positions for the employees whose salaries are above Rs.50,000.</li>
  This results for using select command and return employee names and their positions from EMPLOYEE table where salary > 50000.
<li> List the customer names who registered before 2022-01-01 and have not issued any books yet.</li>
        This results for using select command and return customer names by left joining CUSTOMER and ISSUE table where register date <  2022-01-01.
<li> Display the branch numbers and the total count of employees in each branch.</li>
           This results for using select command and return branch numbers and the total count of employees by joining EMPLOYEE and BRANCH table using group by command.
<li> Display the names of customers who have issued books in the month of June 2023.</li>
         This results for using select command and return names of customers by joining CUSTOMER and ISSUE table where issue date in month june and year is 2023.
<li> Retrieve book_title from book table containing history.</li>
       This results for using select command and return book_title from BOOK table where category is history.

<li> Retrieve the branch numbers along with the count of employees for branches having more than 5 employees</li>
             This results for using select command and return  branch numbers along with the count of employees by joining EMPLOYEE and BRANCH table using group by command and having employee count is greater than 5.

</ol>

###### *Note : The above queries outputs are listed in LibraryManagementSystem.pdf.


## Conclusion

<p>Using the above queries we get the correct results from the DB.So These use of this Mysql queris help to sort out the expected data from this all details</p>



