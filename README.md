# Kristina's Tech Store - Inventory Management System

## 📋 Project Overview
A complete Spring Boot web application for managing computer parts and products inventory. Built for Kristina's Tech Store to track inventory with min/max validation, purchase functionality, and comprehensive part management.

## 🚀 Features
- **Part Management**: Add, update, delete computer parts (Inhouse & Outsourced)
- **Product Management**: Manage assembled computer products with Buy Now functionality  
- **Inventory Validation**: Min/Max inventory tracking with real-time validation
- **Search & Filter**: Find parts and products quickly
- **H2 Database**: Embedded database with web console
- **Responsive UI**: Clean, professional interface

## 🛠️ Technology Stack
- **Backend**: Spring Boot 3.5.7, Java 21
- **Database**: H2 Database (file-based)
- **Frontend**: Thymeleaf, HTML, CSS
- **Testing**: JUnit 5
- **Build Tool**: Maven

## 📁 Project Structure
src/
├── main/
│ ├── java/com/example/cs/
│ │ ├── model/ # Entity classes (Part, InhousePart, OutsourcedPart, Product)
│ │ ├── repository/ # JPA repositories
│ │ ├── service/ # Business logic & sample data
│ │ ├── controller/ # MVC controllers
│ │ └── CsApplication.java
│ └── resources/
│ ├── templates/ # Thymeleaf HTML pages
│ ├── static/css/ # Stylesheets
│ └── application.properties
└── test/


## 🏃‍♂️ How to Run

### Prerequisites
- Java 21
- Maven 3.6+

### Running the Application
```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/kristinas-tech-store-inventory.git
cd kristinas-tech-store-inventory

# Run the application
mvn spring-boot:run

# Access the application
# Main App: http://localhost:8080
# H2 Console: http://localhost:8080/h2-console
H2 Database Connection
JDBC URL: jdbc:h2:file:./data/kristina_tech_inventory

Username: sa

Password: password

📊 Sample Data
The application automatically loads sample data:

5 Computer Parts: Mix of Inhouse and Outsourced

5 Computer Products: Various computer systems

🧪 Testing
bash
# Run all tests
mvn test

# Run specific test
mvn test -Dtest=PartTest
📝 Assignment Requirements Implementation
Part A: Git Repository
✅ GitLab repository created with proper commit history

✅ GitHub repository synchronized

Part B: README File
✅ Comprehensive documentation with change tracking

Part C: Customize User Interface
✅ Shop name: "Kristina's Tech Store"

✅ Computer-specific parts and products

✅ Professional CSS styling

Part D: About Page
✅ Company description and contact information

✅ Navigation between pages

Part E: Sample Inventory
✅ 5 computer parts (Intel Core i7, Corsair RAM, Samsung SSD, etc.)

✅ 5 computer products (Gaming PC, Office Workstation, etc.)

✅ Only loads when database is empty

Part F: Buy Now Button
✅ Added to product list next to update/delete

✅ Decrements product inventory by one

✅ Success/error messages for purchases

Part G: Max/Min Inventory Tracking
✅ Added minInv and maxInv fields to Part entity

✅ Updated forms with min/max input fields

✅ Database file renamed to kristina_tech_inventory

✅ Inventory validation between min and max

Part H: Validation
✅ Error messages for inventory below minimum

✅ Error messages for inventory above maximum

✅ Validation during part add/update operations

Part I: Unit Tests
✅ 2 unit tests in PartTest class

✅ Tests for min/max inventory validation

✅ All tests passing

Part J: Clean Code
✅ Removed unused validator classes

✅ Clean, maintainable code structure

Part K: Professional Communication
✅ Clear documentation

✅ Professional code comments

✅ Proper commit messages

🔧 Code Changes Reference
Part C: Customize UI
index.html (Line 25) - Updated shop name

parts.html (Lines 40-55) - Computer parts names

products.html (Lines 40-55) - Computer products names

Part D: About Page
about.html (Entire file) - Created About page

MainController.java (Lines 35-40) - Added about mapping

Part E: Sample Inventory
DataLoader.java (Lines 30-70) - 5 computer parts and products

Checks for empty database before adding

Part F: Buy Now Button
products.html (Lines 65-70) - Buy Now button

ProductController.java (Lines 50-65) - buyProduct method

Part G: Max/Min Inventory
Part.java (Lines 25-35) - minInv, maxInv fields

part-form.html (Lines 50-65) - Min/max inputs

Part H: Validation
Part.java (Lines 55-75) - Inventory validation

part-form.html (Lines 70-80) - Error messages

Part I: Unit Tests
PartTest.java (Lines 30-55) - 2 tests for min/max validation

👨‍💻 Developer
Your Hardik Hariyani
Java Spring Frameworks - D287

📄 License
This project is for educational purposes as part of WGU coursework.

text

## STEP 3: Additional GitHub Files

**.gitignore** (if not already present)
Maven
target/
pom.xml.tag
pom.xml.releaseBackup
pom.xml.versionsBackup
pom.xml.next
release.properties
dependency-reduced-pom.xml
buildNumber.properties
.mvn/timing.properties

IDE
.idea/
*.iws
*.iml
*.ipr
.classpath
.project
.settings/
bin/

OS
.DS_Store
Thumbs.db

Database
*.db
*.mv.db
data/
└── java/com/example/cs/
└── PartTest.java # Unit tests
