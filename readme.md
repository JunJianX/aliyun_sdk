call mvn -f pom.xml dependency:copy-dependencies

若有多个jar要加入path中，可以用分号“;”间隔，编译时也可以：
javac -cp D:\lab\*.jar Lab.java

javac -cp .;E:\code\maven_project\cloud_sdk\target\dependency\*  E:\code\maven_project\cloud_sdk\src\main\java\com\junjian\demo\AmqpJavaClientDemo.java
java -cp .;E:\code\maven_project\cloud_sdk\target\dependency\* com.junjian.demo.AmqpJavaClientDemo