# VideoCloud

<h1 id="top">------------------------ PORTOFOLIO --------------------------</h2>
 

# introduction
### Individual project
In dit project wil ik een online platform maken waarin gebruikers media van andere gebruikers kunnen beluisteren en zelf ook media kunnen oploaden. Deze media zal alleen muziek zijn. Het doel is om hiermee aan te tonen dat ik kan laten zien dat ik begrijp hoe een JavaScript front-end werkt, dat ik dit kan combineren met een OO gebaseerde back-end taal en dat de software gedistribueerd is zodat het een grote hoeveelheid aan gebruikers tevreden kan stellen. Om dit proces voor de gebruiker zo snel en efficiënt mogelijk te maken zal er gebruik worden gemaakt van asynchrone communicatie om te voorkomen dat een gebruiker lang moet wachten. In combinatie van een intuïtieve UX moet dit ervoor zorgen dat de gebruikservaring van de website zo optimaal mogelijk is. De data van de gebruiker zal opgeslagen worden in een relationele database. Aangezien dit gevoelige informatie is zal er gekeken moeten worden naar verschillende beveiligingsopties om de data van de gebruiker te kunnen beschermen.

### Group project




# Learning outcomes


1. You design and build **user-friendly**, **full-stack** web applications.

2. You use software tooling and methodology that continuously monitors and improve the software quality during software development.

3. You choose and implement the most suitable agile software development method for your software project.

4. You design and implement a (semi)automated software release process that matches the needs of the project context.

5. You recognize and take into account cultural differences between project stakeholders and ethical aspects in software development.

6. You analyze (non-functional) requirements, elaborate (architectural) designs and validate them using multiple types of test techniques.

7. You analyze and describe simple business processes that are related to your project.

8. You act in a professional manner during software development and learning.


##  1. web application

**_Clarification:_**

**_User friendly:_** _You apply basic User experience testing and development techniques._

**_Full-stack:_** _You design and build a full stack application using commonly accepted front end (Javascript-based framework) and back end techniques (e.g. Object Relational Mapping) choosing and implementing relevant communication protocols and addressing asynchronous communication issues._


**1. User with comment list**
I made a users page where the application calls the GetAllUsers() and getCommentsByUser() method and then proceeds to map all the users into rows. As seen below.

![website_users](https://user-images.githubusercontent.com/73832880/171807355-f0c099b5-179d-4760-bba4-a0efd750e124.JPG)

As you can see below, the backend recieves APi calls and processes it into actions.

UserController.java

![java_usercontrollerl](https://user-images.githubusercontent.com/73832880/171807701-4f9e4766-d18f-48c3-b3a2-865954d3ae8d.JPG)

Postman users api call

![musics_postman](https://user-images.githubusercontent.com/73832880/171807830-681119d0-6392-4341-b122-77cfcf7f34c1.JPG)

 ## 2. Software quality

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


## 3. Agile Method

[Agile Methode Document](https://github.com/SandervanDeurzenStudent/VideoCloud_Portofolio/new/main/Leeruitkomsten)

## 4. CI/CD

[CICD Document](https://github.com/SandervanDeurzenStudent/VideoCloud_Portofolio/new/main/Leeruitkomsten/CICD.md)



## 5. Ethics and Cultural differences

**_Clarifications:
Recognize:  Recognition is based on theoretically substantiated awareness of cultural differences and ethical aspects in software engineering.
Take into account:
Adapt your communication, working, and behavior styles to reflect project stakeholders from different cultures; _**

[Ethics Document](https://github.com/SandervanDeurzenStudent/VideoCloud_Portofolio/blob/main/Leeruitkomsten/Ethics.md)
[Cultural Differences Document](https://github.com/SandervanDeurzenStudent/VideoCloud_Portofolio/blob/main/Leeruitkomsten/Cultural_differences.md)



##  6. Requirements and Design

**_Clarification:_**
**_Multiple types of test techniques: You apply user acceptance testing and stakeholder feedback to validate the quality of the requirements. You evaluate the quality of the design (e.g., by testing or prototyping) taking into account the formulated quality properties like security and performance._**



After our first interview with our stakeholder World of Content,  we had an understanding of what the client expects from us. Our group started writing user stories connected to the requirements. We prioritized the user stories by importance. We made concepts, models and designs before we started the development. With every comeback every 3 weeks, we took our time to ask more questions, review our user stories and plans for the future, and noticably tweaked our planning and notes in accordance to the conversations we held with World of Content.
Requirement documents

User stories Group Project

![Piada_userstories](https://user-images.githubusercontent.com/73832880/171812203-60237c05-a8e1-4d1a-b072-580061738972.jpg)

Database model Group Project

![piada_database](https://user-images.githubusercontent.com/73832880/171812105-82ee2a77-871a-4206-941a-45bd50861a08.jpg)



![RequirementsJPG](https://user-images.githubusercontent.com/73832880/171811065-34c3a98c-74d3-46a5-b4df-24190963b0e2.JPG)






## 7. Business processes

**_Clarification:
Simple: Involving stakeholders, predominantly sequential processes with one or two alternative paths.
Related:
Business processes during which the software that you are developing will be used (business processes that the software must support by fully or partially automating them). 
or
Business processes needed for the success of your software development project (e.g., product release, market release, financial assurance).


## 8. Professional

**_Clarification:_**

**_Professional manner:_**

**_You actively ask and apply feedback from stakeholders and advise them on the most optimal technical and design (architectural) solutions.
You choose and substantiate solutions for a given problem. _**

### 1. trelloboard
I chose to make a trelloboard to keep track of al my progression this sprint in my user stories. Every sprint the trelloboard gets updated.

Trelloboard

![Trello_individidueel](https://user-images.githubusercontent.com/73832880/171808826-3bcf451c-cc34-4b5f-adbe-5de2793dda6c.JPG)

### 2. Research documents

Here below you can find the links to my research documents.

[research_XSS](https://github.com/SandervanDeurzenStudent/VideoCloud_Portofolio/blob/main/Research/S3_IP-Research_XSS.docx)

[research H2 Databases](https://github.com/SandervanDeurzenStudent/VideoCloud_Portofolio/blob/main/Research/S3_research_h2database.docx)

[mini research: APi's](https://github.com/SandervanDeurzenStudent/VideoCloud_Portofolio/blob/main/Research/S3_research_API.docx)

Here below you can find the links to my Git repositories.

Individual Project:

[IP-frontend](https://github.com/SandervanDeurzenStudent/s3-videoCloud_FrontEnd)

[IP-backend](https://github.com/SandervanDeurzenStudent/VideoCloud_backend)

Group Project:

[GP-frontend](https://github.com/RensvGemert/S3-GP-Frontend)

[GP-backend](https://github.com/RensvGemert/S3-GP-Backend)

### 3. Git flow

In my project I use the git flow in my source control. The workflow is great for a release-based software workflow.

Branches:

- A main branch is created
- A develop branch is created from main
- Feature branches are created from develop
- When a feature is complete it is merged into the develop branch using Pull Request
- Closing the used feature branch
- When the development branch is done it is merged into main using Pull Request

![Gitkraken_flow](https://user-images.githubusercontent.com/73832880/171828743-8cf2aedd-df84-4819-ae63-42b1f0078926.JPG)
