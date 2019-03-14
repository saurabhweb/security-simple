# security-simple
Spring Boot Web with a very basic InMemory Authentication Provider

A basic barebones project that configures spring security in a web mvc app using an InMemory Authentication Provider.

To run:
1) Clone the project.
2) From the security-simple directory, run
./mvnw spring-boot:run

Open localhost:8080 in a browser.


Changes:
1) mvn eclipse:eclipse

a) Edit .gitignore to allow eclipse classes into git.

2) Added application.yml to change server port and enable logging.
Problem was that spring boot was not picking up my application.yml
Found link on stackoverflow saying mvn eclipse:eclipse is quite broken (https://stackoverflow.com/questions/46354148/spring-boot-eclipse-why-application-properties-is-excluded-in-classpath)

a) Converted eclipse project to Maven project in eclipse. Right-click project -> Configure -> Convert to Maven project

b) Disable resource filtering in pom.xml
