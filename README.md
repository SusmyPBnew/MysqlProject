# MysqlProject
                                                               
    
  ## Library Management System(MySql Project)

  <p>In this project describes about the some sql queries implement to get the data under Library Management System.Library have huge collections of books,so we have to get categorize data using this sql queries</p>

  For writing queries we need to store the data in particular tables,which describes below,

  ## Tables for Storing Library Management Data

<ol>
<li>Branch: This table for storing no of library branches,that including fields like branch_no(<b>primary key</b>), manager_id,branch_address, and contact_no.</li>

<li>Employee: This table for storing employees details working under the these branches,that including fields like employee_id(<b>primary key</b>), name, position, salary, and the branch_no(<b>foreign key</b>).</li>

<li>Books:  This table for storing books deatails that available in all libraries ,that including fields like ISBN(<b>primary key</b>), title, category, rental price,status(we need to set "yes" or "no", author, and publisher.</li>

<li>Customer: This table for storing customer deatails him/her buy a particular book from any library,that including fields like customer_id(<b>primary key</b>), name, address, and registration date.</li>

<li>IssueStatus: This table for storing issued books by customer details,that including fields like issue_id(<b>primary key</b>), customer_id(<b>foreign key</b>), book name, issue date, and ISBN(<b>foreign key</b>).</li>

<li>ReturnStatus: This table for storing retured books by customer details,that including fields like return_id(<b>primary key</b>), customer_id(<b>foreign key</b>), book name, return date, and ISBN(<b>foreign key</b>).</li>
</ol>


###### *Note : PRIMARY KEY specify above, is a column in a relational database table that's distinctive for each record and A FOREIGN KEY is a field (or collection of fields) in one table, that refers to the PRIMARY KEY in another table.

