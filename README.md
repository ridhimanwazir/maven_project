# TicTacToe a java maven project
A simple Java console application for tic-tac-toe

## Requirements

```
java -version
```
```
mvn -v
```

## Project Structure

- src: contains the main and test folders for Java applications.
 1. main/java contains the source code for the application such as the game board, players, moves, etc.
 2. test/java/test contains the test application and various scenarios for testing based on conditions such as invalid configs, invalid move types, invalid board configs, etc.
- pom.xml: defines all the project configurations, dependencies, plugins, etc.
- config.properties: defines sample configurations users need to provide to start the game

## Building the application : 
after cloning the repository go to the main folder which contains the `pom.xml` file and run 
```
mvn clean install
```

## Running the JAR :
* After having a successful build you should have a `target` folder containing the JAR file `tic-tac-toe-0.0.1.jar`
make sure the JAR file is executable 
if it is not executable you can use the command 
```
chmod +x tic-tac-toe-0.0.1.jar
``` 


* Download a sample `config.properties` file from [here](https://github.com/ridhimanwazir/maven_project/blob/main/config.properties) and put it in the same folder of the JAR file `target` 


* Run the JAR file using the command : 
```
java -jar tic-tac-toe-0.0.1.jar ./config.properties
```

and play !!!!


**Note**: If you don't pass a configuration file path as an argument or an invalid configuration file you will get an error according to what went wrong and the application will not run.


## Running the tests : 
to run the tests use 
```
mvn test
``` 
