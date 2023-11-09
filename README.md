# Student Management System (Golang)

This is a student management system built using Golang, GORM (a popular Object-Relational Mapping library for Golang), and Echo (a fast and unfancy HTTP server framework for Go). This project allows you to manage students' information efficiently, including their details, courses, and grades.

## Features

- **Student Management:** Add, update, view, and delete student records.
- **Course Management:** Manage different courses offered in the institution.
- **Grade Management:** Assign and manage grades for students in various courses.

## Prerequisites

- Go (version 1.15 or higher)
- GORM (Golang Object Relational Mapping) - Ensure it is properly installed (`go get -u github.com/jinzhu/gorm`)
- Echo - HTTP router and middleware framework for Go (`go get -u github.com/labstack/echo/v4`)

## Installation

1. Clone the repository:

   ```
   git clone https://github.com/shaunakdas/go-student-management-system.git
   ```

2. Change directory to the project folder:

   ```
   cd student-management-system
   ```

3. Install dependencies:

   ```
   go get ./...
   ```

4. Run the application:

   ```
   go run main.go
   ```

5. Access the application in your web browser at `http://localhost:8080`.

## Database Configuration

This project uses a MySQL database by default. Update the database configuration in the `config.go` file with your own database credentials:

```go
var (
	DBUsername = "your-username"
	DBPassword = "your-password"
	DBHost     = "localhost"
	DBPort     = "3306"
	DBName     = "student_management"
)
```

## API Endpoints

- **GET /students:** Get a list of all students.
- **GET /students/:id:** Get details of a specific student by ID.
- **POST /students:** Add a new student.
- **PUT /students/:id:** Update details of a student by ID.
- **DELETE /students/:id:** Delete a student by ID.
- **GET /courses:** Get a list of all courses.
- **GET /courses/:id:** Get details of a specific course by ID.
- **POST /courses:** Add a new course.
- **PUT /courses/:id:** Update details of a course by ID.
- **DELETE /courses/:id:** Delete a course by ID.
- **GET /grades:** Get a list of all grades.
- **GET /grades/:id:** Get details of a specific grade by ID.
- **POST /grades:** Add a new grade.
- **PUT /grades/:id:** Update details of a grade by ID.
- **DELETE /grades/:id:** Delete a grade by ID.

## Contributors

- [Your Name](https://github.com/Shaunakdas)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

Feel free to contribute and report issues! Happy coding!