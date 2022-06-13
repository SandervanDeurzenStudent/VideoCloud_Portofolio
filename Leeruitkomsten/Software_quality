**_Clarification:_**

**_Tooling and methodology:_** _Carry out, monitor and report on unit integration, regression and system tests, with attention for security and performance aspects, as well as applying static code analysis and code reviews._

### 1. Unit and integration tests
For this learning outcome I made some unit and integration tests. This will verify that my application is doing what it's supposed to do. Also a good benefit of testing is preventing bugs and helps with the quality of the code. On the images below you can see two sort of tests I made: unit and integration tests. Here is some explanation on both of these tests.

`Unit testing:`  This is a testing technic that tests individual units of code (methods). So for example in my application, one test will only test the method that gives me all the products, and another may test the method that can create a product. It's possible for the developer to use mockobjects to simulate behaviors of objects. This is helpfull when you are testing because you can use fake objects instead of the real objects from your project.

`Integration testing:`  With integration testing the entire process in tested (in this case a specific request). This is done with MockMvc. MockMvc allows you to send fake HTTP requests to a controller and test how the controller behaves. A good way to test these request is with fake data so when you want to create a new product for example you already tested the request with fake product data that you made up. This way you can test the entire application process.

Integration tests

![productControllertestsJPG](https://user-images.githubusercontent.com/73832880/171404379-19d5b2cd-3c5e-421b-b315-1630a234a7ff.JPG)


unit tests

![unitTests](https://user-images.githubusercontent.com/73832880/172367686-05295f9a-c0eb-4bd2-8722-d61510045393.JPG)


### 2. Testing with H2 database
A good reason to use an H2 database is because it can be configured to run as in-memory database. The benefits of this are that it can create a clean database, execute unit tests and then delete the database very fast. If you would create and delete a physical database at each build it would consume much time. On the images below you can see that i setup some properties and that i run the unit tests with the H2 database. Also the tests run very fast.

Configuration of the H2 database:

Properties

![testdatabase_properties](https://user-images.githubusercontent.com/73832880/171404078-d6d84e7a-4c25-443a-be69-43530e57e11f.JPG)

H2 test Database insert

![database_insert_test](https://user-images.githubusercontent.com/73832880/171404102-a41edcec-f10e-4ca7-8960-b8b63d3e4b4a.JPG)


Testing with H2 database

![productControllertestsJPG](https://user-images.githubusercontent.com/73832880/171402420-27b30788-1d76-4621-b90c-442714339fb6.JPG)


### 3. Code scans
My project uses the github workflow Sonarcloud. On every push Sonarcloud fully scans my code for errors, typing mistakes and vulnerabilities in my code.

![sonarcloud](https://user-images.githubusercontent.com/73832880/171404141-331a828b-a0ea-4914-917b-7e7587d72af1.png)

