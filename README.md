# EVIS ERP Software

A multi-module web-based ERP built as an M.Sc. project at the People's University of Bangladesh, submitted on 25 October 2019.

## About

EVIS ERP brings the core operations of a small business — planning, manufacturing, inventory, sales, staff, finance and customer communication — into one application on a single MySQL schema.

- **Programme:** M.Sc. in Computer Science and Engineering
- **Institution:** The People's University of Bangladesh, Department of CSE, Dhaka
- **Supervisor:** Mrs. Husne Farah, Lecturer, Department of CSE
- **Co-author:** Ashif Md. Ibran Hossain
- **Submitted:** 25 October 2019

The project was submitted jointly. This is the copy I retained and continued to develop afterwards; the point-of-sale and e-commerce storefront modules were added in November and December 2019 and are not part of the submitted book.

## Modules

The submitted system covers fifteen modules:

1. Product planning
2. Manufacturing
3. Service (after-sales)
4. Inventory management
5. Marketing campaigns
6. Customer / shop manager
7. Supplier manager
8. Employee manager
9. Salary manager
10. Cashbook
11. Income manager
12. Expense manager
13. Internal email
14. Payment manager
15. Chat

## Repository layout

```
application/   controllers, models, views and config
system/        CodeIgniter 2.2.6
img/           product, employee, shop and supplier images
public/        CSS, JavaScript and plugins
index.php      front controller
```

The database schema is **not** included; the dump is retained offline.

## Stack

- PHP 7.x on CodeIgniter 2.2.6
- MySQL (31 tables)
- HTML, CSS (Bootstrap), JavaScript (jQuery)
- XAMPP for local development

## Design

Built with the waterfall model: requirements, design, implementation, testing, integration, maintenance. The design work is documented in the project book — entity-relationship diagrams, data-flow diagrams and a normalised relational schema (chapters 4 and 5), with the interface and results in chapter 6.

## Running it

1. Create a MySQL database and import a schema of your own; the original dump is not in this repository.
2. Set the database name, user and password in `application/config/database.php`.
3. Point Apache at the project root and open `index.php`.

CodeIgniter 2.2.6 is end-of-life and the code targets PHP 7.x. It will not run unmodified on current PHP.

## Limitations

This is a student project, not a production system. There are no users, revenue or adoption claims. The code is preserved as it was written in 2019–2020, not refactored for current PHP versions, and the repository is not maintained.

## Third-party code

CodeIgniter, dompdf, Bootstrap and jQuery are included under their own licences; those licences remain with their authors.
