# Library-management-system
The Library Management System is a comprehensive database project designed to manage all aspects of library operations. It helps track books, employees, customers, and the status of book issues and returns. The system organizes library data in six key tables: Branch, Employee, Books, Customer, IssueStatus, and ReturnStatus.

This project enables efficient management of library resources, making it easier to query and manage the inventory, customer information, and employee details.

Project Structure
The project consists of the following tables:

1. Branch
Contains information about library branches.

Branch_no (PRIMARY KEY)
Manager_Id
Branch_address
Contact_no
2. Employee
Contains information about employees working at the library.

Emp_Id (PRIMARY KEY)
Emp_name
Position
Salary
Branch_no (FOREIGN KEY, refers to Branch_no in Branch table)
3. Books
Contains information about books available in the library.

ISBN (PRIMARY KEY)
Book_title
Category
Rental_Price
Status (Available: Yes/No)
Author
Publisher
4. Customer
Contains information about customers who have registered with the library.

Customer_Id (PRIMARY KEY)
Customer_name
Customer_address
Reg_date
5. IssueStatus
Tracks the status of books that have been issued.

Issue_Id (PRIMARY KEY)
Issued_cust (FOREIGN KEY, refers to Customer_Id in Customer table)
Issued_book_name
Issue_date
ISBN_book (FOREIGN KEY, refers to ISBN in Books table)
6. ReturnStatus
Tracks the status of books that have been returned.

Return_Id (PRIMARY KEY)
Return_cust
Return_book_name
Return_date
ISBN_book2 (FOREIGN KEY, refers to ISBN in Books table)
