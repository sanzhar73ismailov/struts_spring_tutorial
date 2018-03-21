
rem example from https://www.eclipse.org/jetty/documentation/9.3.x/advanced-embedding.html

rem Use curl as follows:
curl -o jetty-all-uber.jar http://central.maven.org/maven2/org/eclipse/jetty/aggregate/jetty-all/9.3.23-SNAPSHOT/jetty-all-9.3.23-SNAPSHOT-uber.jar

rem The following command compiles the HelloWorld class:
javac -d classes -cp jetty-all-uber.jar HelloWorld.java

rem The following command runs the HelloWorld example:
java -cp classes;jetty-all-uber.jar org.eclipse.jetty.embedded.HelloWorld

You can now point your browser at http://localhost:8080 to see your hello world page.