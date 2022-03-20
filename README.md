# JavaStuff
All learnings related to Java

# To compile and run with external dependency
```sh
javac -classpath external.jar com/mycompany/myClass.java
java -classpath external.jar com.mycompany.myClass
# Or if not in any package
java -cp .;json-java.jar Test (Windows)
java -cp .:json-java.jar Test (Unix Systems)
```

# Create and running Jar
```sh
jar cf jar-file-name.jar Test.class
# To automatically update MANIFEST.MF with Main-Class: classname
jar cfe jar-file-name.jar Test Test.class
# WAY1: Call java with the main class and add jar files, including your json-20211205.jar, on the command line
java -cp json-20211205.jar:jar-file-name.jar Test
# WAY2: Include dependencies in json-20211205.jar's manifest file (and then run java -jar)

```
