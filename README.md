# StudentsManagementSystem

📚 Student Management System (CRUD Application)

A simple, robust web application built using Spring Boot to manage student records. It allows for seamless Create, Read, Update, and Delete (CRUD) operations, powered by dynamic HTML rendering via Thymeleaf.✨ FeaturesView All Students: Displays a paginated list of all students currently in the database.Add New Student: Provides a form for creating and saving new student records.Update Student: Allows editing of existing student information.Delete Student: Removes a student record from the database.Thymeleaf Templating: Utilizes Thymeleaf for clean, server-side rendered HTML views.💻 Technologies UsedTechnologyDescriptionJavaCore programming language.Spring BootFramework for rapid application development and setup.Spring Data JPAUsed for database persistence and repository management.ThymeleafModern server-side Java template engine for dynamic HTML.MySQL / H2Database of choice (specify which one you used).Maven / GradleDependency management and build tool (specify which one you used).🚀 Getting StartedFollow these instructions to get a copy of the project up and running on your local machine.PrerequisitesJava 17+ (or the version you used)Maven (or Gradle)An IDE (e.g., IntelliJ IDEA, VS Code, Eclipse)Installation & SetupClone the repository:Bashgit clone [Your Repository URL Here]
cd Student_management_sys_java
Configure the Database:If using MySQL, update the database connection details in src/main/resources/application.properties (or application.yml).Properties# Example for MySQL
spring.datasource.url=jdbc:mysql://localhost:3306/student_db
spring.datasource.username=root
spring.datasource.password=password
spring.jpa.hibernate.ddl-auto=update
(Note: If you used H2 for simplicity, no changes are required!)Run the application:Using Maven:Bashmvn spring-boot:run
Using Gradle:Bash./gradlew bootRun
Access the application:The application will start on port 8080. Open your web browser and navigate to:http://localhost:8080/students
📂 Project StructureThis is a typical Spring Boot project layout:Student_management_sys_java/
├── src/main/java/com/example/studentmgmt/
│   ├── controller/   # Handles web requests (e.g., StudentController)
│   ├── model/         # Data models (e.g., Student.java)
│   ├── repository/    # Database interaction (e.g., StudentRepository)
│   └── service/       # Business logic layer (e.g., StudentService)
└── src/main/resources/
    ├── static/        # CSS, JavaScript, Images
    ├── templates/     # Thymeleaf HTML templates (*.html)
    └── application.properties # Configuration files
🤝 ContributionContributions are welcome! If you have suggestions or find a bug, please open an issue or submit a pull request.
