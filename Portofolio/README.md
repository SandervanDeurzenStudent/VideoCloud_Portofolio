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

**_ Clarification:_**
**_Choose :You are aware of the most popular agile methods and their underlying agile principles. Your choice of a method is motivated and based on well-defined selection criteria and context analyses.**_



***"Agile methods or Agile processes generally promote a disciplined project management process that encourages frequent inspection and adaptation, a leadership philosophy that encourages teamwork, self-organization and accountability, a set of engineering best practices intended to allow for rapid delivery of high-quality software, and a business approach that aligns development with customer needs and company goals."*** https://www.cprime.com/resources/what-is-agile-what-is-scrum/#:~:text=Agile%20methods%20or%20Agile%20processes,rapid%20delivery%20of%20high%2Dquality

To work as efficient as possible in our group, we made sure to keep our proces and tasks on a scrumboard. We used a trelloboard to help us with that as you can see below. 

![Trello](https://user-images.githubusercontent.com/73832880/171404156-8d70eb2d-52a0-4572-bd14-031f62f39563.png)

Our user stories that we set up this project consist out of multiple properties. As you can see below the user story contains a timestamp, labels, checklists and members connected to it. This way we can see well-organized what the user stories are and which tasks everyone is working on.

![image](https://user-images.githubusercontent.com/73832880/171827420-08b33c91-4ca7-4730-b8dc-e0e433032e71.png)



## 4. CI/CD

**_Clarification:
Design and implement: You design a release process and implement a continuous integration and deployment solution (using e.g. Gitlab CI and Docker).
_**

### 1. docker
Docker allows developers to make lightweight containers of their application that can be run virtually anywhere. I use a Github workflow package called Docker Publish which automaticly creates images on pushes to master. 


 docker container 
 
![DockerContainers](https://user-images.githubusercontent.com/73832880/171404191-8f0ca376-d4eb-4f15-ae36-935fb3d14014.JPG)

Docker images

![DockerImages](https://user-images.githubusercontent.com/73832880/171404264-3d343cc3-ab7a-4165-958b-0b5650dff166.JPG)


My Backend, Frontend and database are running in docker containers. This is configurated by a .yaml file as seen below.

docker-compose.yaml

![compose_yaml](https://user-images.githubusercontent.com/73832880/171404230-74161da8-40a6-402f-b004-d2498c88fdb7.png)



### 2. automatic testing

By making tests you can check if everything works as it's supposed to, Therefore it might be a good idea to run those test everytime you make a change, as in a push. The code below ensures that with every push to the master branch, every test gets run.

maven.yaml

![mavenyaml](https://user-images.githubusercontent.com/73832880/171806833-17507762-d140-4ed3-8b02-90f4510ac7fd.JPG)


Github Workflows for CI and CD

![workflows_github](https://user-images.githubusercontent.com/73832880/171806983-fa7448de-9d35-4321-9a88-787f267ba9ac.JPG)



## 5. Ethics and Cultural differences

**_Clarifications:
Recognize:  Recognition is based on theoretically substantiated awareness of cultural differences and ethical aspects in software engineering.
Take into account:
Adapt your communication, working, and behavior styles to reflect project stakeholders from different cultures; _**

### 5.1. Ethics

As a software engineer you need to be conscious of the different ethical aspects, principles, and practices within the field. You should ensure that your software meets accessibility standards, that it respects a user's privacy, and that it is secure, amongst other things. In order to achieve this you have to critically evaluate your software design in all stages of its development, starting off with an ethically sound design and adjust it when necessary. I have done research on this subject and performed an ethical analysis of my group project and individual project in order to increase my proficiency at this learing outcome

#### Why are ethics important in software engineering?
Ethics are important in software engineering because the software that an engineer writes has the potential to be used by large groups of people and might have a significant impact on their lives. As a software engineer you have to be aware and mindful of these possible consequences as you envision, develop and deploy your software. Not all consequences can be foreseen but you should feel responsible for attempting to ensure that your software does not cause harmful effects but instead benefits the people who use it.

#### What do you have to do as a software engineer to address ethical aspects in your work?
As a software engineer you need to be aware of the different ethical aspects, principles, and practices within the field. You should ensure that your software meets accessibility standards, that it respects a user's privacy, that it is secure, and all the other aspects as mentioned earlier in this document. In order to achieve this you have to critically evaluate your software design in all stages of its development, starting off with an ethically sound design and adjust it when necessary. Test and review your software frequently to see if it still meets your ethical requirements. Request user feedback and see if their needs are being met, and collaborate with them to improve your software.

#### How do you know that your ethical considerations match with those of other software engineers?
In order to make sure that your ethical considerations match with those of other software engineers like your colleagues, it is advisable to discuss these considerations when starting development of a new software project, as well as when welcoming a new member to the team. Good communication is key, ask your colleagues about their views on the subject and which ethical considerations they find important. It is also a good idea to monitor developments in the field by reading articles (on the internet) and attending conferences about software development.

### 5.2. Cultural differences

For the subject of cultural differences I have done some research about what culture is and what well-known aspects on cultural differences are. I have also written about my personal experiences with cultural differences. This product helps prove my proficiency at this learning outcome.


As a software engineer you will meet all types of different people all over the world with all different types of different cultural standarts. This can lead to conflicts between you and the people you are working with/for. It is therefore important to be aware of these differences so that these intercultural collaborations may proceed smoothly.

#### what is culture?

> Culture is the characteristics and knowledge of a particular group of people, encompassing language, religion, cuisine, social habits, music and arts.
https://www.livescience.com/

#### How does culture affect Businesses?
Most businesses try to improve their image to all cultures and groups around the world to reach more possible customers and come over as user-friendly as possible. Take pride month as an example.  


TICT
![culural_differences](https://user-images.githubusercontent.com/73832880/172370513-34897d4c-953c-47cb-b86f-c2b6182bcc1a.jpg)


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
