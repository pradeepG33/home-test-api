# Karate API Testing Project – Inventory App

This project automates API test scenarios using the Karate BDD testing framework.

1. Prerequisites
Make sure the following are installed:

Java JDK (version 8 or above)
Apache Maven
Git
Docker
An IDE or text editor (like IntelliJ, VS Code, etc.)

2. Run the API with Docker
 Pull the Docker image (only needs to be done once):
  docker pull automaticbytes/demo-app 

 Run the Docker container:
  docker run -p 3100:3100 automaticbytes/demo-app
  
Test the API is live: Open your browser and go to:
  http://localhost:3100/api/inventory
  You should see JSON data of menu items.

3. Create Karate Maven Project ( or) Clone this project from git repository
  1. create a maven project 
  2. add dependencies in pom.xml like karate dependency etc.
  3. Create a karate feature file with scenarios mentioned. 
       i. Get all menu items
       ii.Filter by id
       iii.Add item for non existing id
       iv.Add item for existent id
       v.Try to add item with missing information
       vi.Validate recent added item is present in the inventory
  4. Create a Runner Class
  
4. Go to Maven - Update the Project, mvn clean and run mvn test(executes all scenarios in the project)
5. you can see the status/test results in console
6. A report will be generated in target/karate-reports
