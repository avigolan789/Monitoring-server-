# Monitoring-server-
Devops project 

Part 1 - DevOps Automatic Monitoring Server 
Objective: 
The objective of this part is to create a web server using the Spring Boot framework, a controller, and 
an H2 database. You will also use Maven to automate the project build, emphasizing the DevOps 
practices of automation and consistency. 
Tasks: 
1. Web Server and Controller Setup: Use Spring Boot to create a web server. Define a controller 
with two routes for GET requests. 
• First Route: localhost:8080/logs - This should display all logs in the server. 
• Second Route: Define a route to create a new transaction. 
2. Database Integration: Integrate an H2 database (or any other database you prefer) with your 
server. The logs should be maintained in the database. Each time a GET request is sent from 
the client to the server, a new log should be registered. The log entry should be a string that 
includes the current time, date, and the route through which the request was made. 
3. Automating with Maven: Use Maven to automate the build process of your project. 
4. Seed Class: Create a seed class such that when the server starts, there will be one log that 
includes the time the seed class was invoked or the server started. 
Feel free to declare any POJO, controller, and other classes you'd like, as well as interfaces. Use 
whatever libraries are necessary. 
Relevant DevOps Topics: 
Software Lifecycle, DevOps Tools, Database Management, Infrastructure as Code, Version Control, 
Monitoring and Logging 
Part 2 – Version Control and GitHub 
Objective: 
The objective of this part is to use GitHub to manage your project's source code and track your 
progress over time. 
Tasks: 
1. Setting up a GitHub Repository: 
• Create a new GitHub repository for your project. 
• This repository should contain all your project files, including your source code, your 
Maven configuration file (pom.xml), and your README file. 
2. Version Control: 
• Commit your changes to the repository regularly. Each commit should have a clear 
and descriptive message stating what changes were made. 
• Use branches for developing new features or fixing bugs. Once the work is complete 
and tested, merge it back into the main branch. 
Part 3 – Automated testing with Python  
Objective: 
The objective of this part is to write tests for the web server you created in Part 1 using Python. This 
will allow you to ensure that your web server is functioning correctly, and to find and fix any bugs or 
issues that may arise. 
Tasks: 
1. Python Test Scripts: Write Python scripts to test the functionality of your web server. Your 
scripts should make HTTP requests to the routes served by your Spring Boot application and 
validate the responses. 
• For the localhost:8080/logs route, write a test to ensure that the page returns the 
expected logs. This should include checking the status code, the response format, and 
the content of the response. 
• For the second route that creates a new transaction, write a test to ensure that a new 
log is created each time a GET request is made. Again, this should include checking 
the status code, the response format, and the content of the response. 
2. Error Handling: Your tests should include error handling. If an HTTP request returns an error, 
your script should be able to catch that error and return a useful error message. 
Bonus - Python BDD: 
For bonus points, you can use a Python BDD (Behavior-Driven Development) framework such as 
Behave or Cucumber to write your tests. 
BDD is a software development approach that emphasizes collaboration between developers, QA and 
non-technical or business participants in a software project. It encourages teams to use conversation 
and concrete examples to formalize a shared understanding of how the application should behave. 
You will need to write Gherkin scenarios that describe the behavior of your web server, and then 
implement step definitions in Python that execute those scenarios against your server. 
Remember, the goal of these tests is to ensure that your server behaves as expected when it receives 
various types of HTTP requests. BDD can help clarify what those expectations are and ensure that 
everyone on the team has the same understanding.
