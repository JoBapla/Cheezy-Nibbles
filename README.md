# CMPT276 - Final Project (Group 6)

## Maven-getting-started

### Install Apache Maven
- Make sure to have Apache Maven installed on your system
    - A detailed explanation and installation guide[ here](https://maven.apache.org/install.html "This link takes you to Apache Maven installation guide!")
- If Maven is already installed, skip this step

## How To Run Game

```sh
$ git clone git@csil-git1.cs.surrey.sfu.ca:group-6/project.git
$ cd project
$ mvn clean
$ mvn package
```
wait till build is finished
```sh
$ cd target/
$ java -jar untitled-1.0-SNAPSHOT.jar 
```

## How To Test Game

### Set up Test Environment
- Change directory to the maven project:
```sh
$ cd project
```

- Inside the project folder, there should be the pom.xml file
- This file needs to be present for maven to test the project
- All maven dependencies are in the pom.xml

### Run Tests
- Make sure you are in the directory with the pom.xml file
- To run all tests in the maven project, execute this line:
```sh
$ mvn test
```
- To run individual tests:
```sh
$ mvn -Dtest=<Insert test name> test
```
- All individual test classes are found below
- Copy and paste a name into the "insert test name" field without the "<>" brackets
- For example:
```sh
$ mvn -Dtest=CharacterTest test
```

### Individual Test Classes
- CharacterTest
- EnemyTest
- HeroTest
- UtilTest
- ImageLoaderTest
- GameTimeTest
- GraphicTest
- EndLoseScreenTest
- EndWinScreenTest
- MapTest

### Documentation
- For more information on Apache maven
    - [Apache Maven](https://maven.apache.org/what-is-maven.html "This link takes you to Apache Maven")