# My Second project in Java - DAO (Data Access Object) JDBC 

This is my second project done in Java, you can notice that I have progressed a bit in the language since my first project (chess system). This project is more about learning how JDBC works and also DAO.
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






















###### Again, I would like to thank Professor Nélio Alves for sharing his brilliant knowledge with the course subscribers. It's been a perfect journey, and I learn a lot from him.