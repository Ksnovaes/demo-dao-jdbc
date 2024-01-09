# My Second project in Java - DAO (Data Access Object) JDBC 

This is my second project done in Java, you can notice that I have progressed a bit in the language since my [first project (chess system)](https://github.com/Ksnovaes/chess-system-java/). This project is more about learning how JDBC works and also DAO.
I am glad to see that I am advancing more and more in my projects.

###### I confess that I found this project now easier than the first one because the first one involved a lot of logic, but with a bit of study, you start to understand more clearly.

## Checklists:
> **#1 - Creating project and git repository**
- [x] GitHub: create a new project
- [x] Add external library in Intellij
> **#2 - Department entity class**
- [x] Entity class checklist:
  - Attributes
  - Constructors
  - Getters/Setters
  - hashCode & equals
  - toString
  - implements Serializable
> **#3 - Seller entity class**
- [x] Entity class checklist:
  - Attributes
  - Constructors
  - Getters/Setters
  - hashCode & equals
  - toString
  - implements Serializable
> **#4 - DepartmentDao & SellerDao interfaces**
- [x] Entity interface checklist:
  - insert() - void
  - update() - void
  - deleteById() - void
  - findById() - Department & Seller
  - findAll - List<Department & Seller>
> **#5 - SellerDaoJDBC and DaoFactory**
- [x] Create SellerDaoJDBC (src.model.dao.impl)
- [x] Create DaoFactory (src.model.dao)
> **#6 - findById implementation**
- [x] findById implementation checklist:
  - SQL Query:
  ``SELECT seller.*,department.Name as DepName
    FROM seller INNER JOIN department
    ON seller.DepartmentId = department.Id
    WHERE seller.Id = ?``
  - If statement to return seller obj (if true)
  - Exceptions
> **#7 - findByDepartment implementation**
- [x] findByDepartment implementation checklist:
  - SQL Query:
  ``SELECT seller.*,department.Name as DepName
    FROM seller INNER JOIN department
    ON seller.DepartmentId = department.Id
    WHERE DepartmentId = ?
    ORDER BY Name``
  - If statement to return seller obj (if true)
  - Exceptions
> **#8 - findAll implementation**
- [x] findAll implementation checklist:
  - SQL Query:
  ``SELECT seller.*,department.Name as DepName
    FROM seller INNER JOIN department
    ON seller.DepartmentId = department.Id
    ORDER BY Name``
  - If statement to return seller obj (if true)
  - Exceptions
> **#9 - Insert implementation**
- [x] Insert implementation checklist:
  - SQL Query:
  ``INSERT INTO seller
    (Name, Email, BirthDate, BaseSalary, DepartmentId)
    VALUES
    (?, ?, ?, ?, ?)``
  - Exceptions
> **#10 - Update implementation**
- [x] Update implementation checklist:
  - SQL Query:
  ``UPDATE seller
    SET Name = ?, Email = ?, BirthDate = ?, BaseSalary = ?, DepartmentId = ?
    WHERE Id = ?``
  - Exceptions
> **#11 - Delete implementation**
- [x] Delete implementation checklist:
  - SQL Query:
  ``DELETE FROM seller
    WHERE Id = ?``
  - Exceptions
> **#12 - DepartmentDao implementation and test**
- [x] DepartmentDaoJDBC
- [x] DaoFactory (createDepartmentDao)
- [x] Test Program2 with department implementations

###### Again, I would like to thank Professor [Nélio Alves](https://www.udemy.com/course/java-curso-completo/#instructor-1) for sharing his brilliant knowledge with the course subscribers. It's been a perfect journey, and I learn a lot from him.