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

# Create jar
```sh
jar cf jar-file-name.jar Test.class
# To automatically update MANIFEST.MF with Main-Class: classname
jar cfe jar-file-name.jar Test Test.class
```
