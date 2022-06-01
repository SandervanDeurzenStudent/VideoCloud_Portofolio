# VideoCloud

<h1 id="top">------------------------ PORTOFOLIO --------------------------</h2>
 

# introductie
In dit project wil ik een online platform maken waarin gebruikers media van andere gebruikers kunnen beluisteren en zelf ook media kunnen oploaden. Deze media zal alleen muziek zijn. Het doel is om hiermee aan te tonen dat ik kan laten zien dat ik begrijp hoe een JavaScript front-end werkt, dat ik dit kan combineren met een OO gebaseerde back-end taal en dat de software gedistribueerd is zodat het een grote hoeveelheid aan gebruikers tevreden kan stellen. Om dit proces voor de gebruiker zo snel en efficiënt mogelijk te maken zal er gebruik worden gemaakt van asynchrone communicatie om te voorkomen dat een gebruiker lang moet wachten. In combinatie van een intuïtieve UX moet dit ervoor zorgen dat de gebruikservaring van de website zo optimaal mogelijk is. De data van de gebruiker zal opgeslagen worden in een relationele database. Aangezien dit gevoelige informatie is zal er gekeken moeten worden naar verschillende beveiligingsopties om de data van de gebruiker te kunnen beschermen.


# Leeruitkomsten



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

IMAGE

 ## 2. Software quality

**_Clarification:_**

**_Tooling and methodology:_** _Carry out, monitor and report on unit integration, regression and system tests, with attention for security and performance aspects, as well as applying static code analysis and code reviews._

### 1. Unit and integration tests
For this learning outcome I made some unit and integration tests. This will verify that my application is doing what it's supposed to do. Also a good benefit of testing is preventing bugs and helps with the quality of the code. On the images below you can see two sort of tests I made: unit and integration tests. Here is some explanation on both of these tests.

`Unit testing:`  This is a testing technic that tests individual units of code (methods). So for example in my application, one test will only test the method that gives me all the products, and another may test the method that can create a product. It's possible for the developer to use mockobjects to simulate behaviors of objects. This is helpfull when you are testing because you can use fake objects instead of the real objects from your project.

`Integration testing:`  With integration testing the entire process in tested (in this case a specific request). This is done with MockMvc. MockMvc allows you to send fake HTTP requests to a controller and test how the controller behaves. A good way to test these request is with fake data so when you want to create a new product for example you already tested the request with fake product data that you made up. This way you can test the entire application process.

Integration tests

IMAGE

unit tests

Image

### 2. Testing with H2 database
A good reason to use an H2 database is because it can be configured to run as in-memory database. The benefits of this are that it can create a clean database, execute unit tests and then delete the database very fast. If you would create and delete a physical database at each build it would consume much time. On the images below you can see that i setup some properties and that i run the unit tests with the H2 database. Also the tests run very fast.

Configuration of the H2 database

IMAGE
![image](https://imgur.com/7JSNiUd)

Testing with H2 database

IMAGE

### 3. Code reviews
My project uses the github workflow Sonarcloud. On every push Sonarcloud fully scans my code for errors, typing mystakes and vulnuralbilties in my code.

IMAGE

## 3. Agile Method



## 4. CI/CD

### 1. docker
Docker allows developers to make lightweight containers of their application that can be run virtually anywhere. I use a Github workflow package called Docker Publish which automaticly creates images on pushes to master. 


 docker container 
IMAGE

My Backend, Frontend and database are running in docker containers. This is configurated by a .yaml file as seen below.

docker-compose.yaml

IMAGE


### 2. automatic testing

By making tests you can check if everything works as it's supposed to, Therefore it might be a good idea to run those test everytime you make a change, as in a push. The code below ensures that with every push to the master branch, every test gets run.

tests.yaml

IMAGE

## 5. Cultural differences

##  6. Requirements and Design

## 7. Business processes

## 8. Professional



# Links
Here below you can find the links to my research documents.

**Research XSS:**
[research_XSS](www.google.com)
**Research:**
[research](www.google.com)

Here below you can find the links to my Git repositories.

**Research XSS:**
[research_XSS](www.google.com)
**Research:**
[research](www.google.com)
