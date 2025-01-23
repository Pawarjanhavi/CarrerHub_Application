# **Job Board Application**

**CareerHub** is a digital platform designed to facilitate job searching and recruitment. It enables job seekers, companies, and recruiters to interact seamlessly by allowing **job posting, profile creation, and job application submission**. This project implements **object-oriented principles, SQL integration, and robust exception handling**.

## **Key Features**

### **Entity Classes**
- **JobListing**: Handles job attributes like `JobID`, `JobTitle`, `JobDescription`, `Salary`, etc.
- **Company**: Manages company details and job postings.
- **Applicant**: Enables profile creation and job applications.
- **JobApplication**: Tracks applications submitted by applicants.

### **Core Functionalities**
- **Apply for Jobs**: Applicants can apply to jobs using their ID and a cover letter.
- **Post Jobs**: Companies can post jobs with details like salary, location, and job type.
- **Retrieve Data**: Fetch lists of jobs, companies, applicants, and job applications.

## **Database Management**
- **Schema Initialization**: Database schema with tables for `Jobs`, `Companies`, `Applicants`, and `Applications`.
- **SQL Integration**: Manage and retrieve data seamlessly.

## **Exception Handling**
- **Invalid Email Format**: Ensures valid email format during applicant registration.
- **Salary Validation**: Handles cases where salaries are negative or invalid.
- **File Upload Errors**: Manages issues like unsupported file formats and size limits.
- **Application Deadlines**: Prevents submissions after the deadline.
- **Database Connection**: Handles database connectivity and query-related exceptions.

## **Database Connectivity**
- **Retrieve Job Listings**: Display attributes like job titles, company names, and salaries.
- **Insert Data**: Manage job postings, applicant profiles, and job applications.
- **Query Salary Range**: Search job listings within a specific salary range.

## **Directory Structure**
- **entity/model**: Contains entity classes without business logic.
- **dao**: Includes interfaces/abstract classes for database interactions and their implementations.
- **exception**: Custom exceptions for handling errors gracefully.
- **util**:
  - **DBPropertyUtil**: Returns the connection string from a property file.
  - **DBConnUtil**: Creates a database connection using the connection string.
- **Main**: Contains the `MainModule` for a menu-driven application demonstrating functionalities.

## **Technical Highlights**
- **Object-Oriented Programming**: Encapsulation, inheritance, and modularity ensure code reusability.
- **SQL Integration**: Class attributes map directly to database column names, simplifying data management.
- **Error Handling**: Comprehensive exception handling ensures smooth and user-friendly operation.
- **Modularity**: The code structure promotes scalability and maintainability.

## **How to Run**
1. Clone the repository and set up the database schema using the provided SQL scripts.
2. Configure the database connection in the property file.
3. Build and run the project in your IDE (e.g., Visual Studio).
4. Use the menu-driven application in `MainModule` to interact with the platform.

## **Sample Use Cases**
- Retrieve all job listings from the database.
- Allow applicants to create profiles and apply for jobs.
- Enable companies to post new job openings.
- Search jobs within a specified salary range.
