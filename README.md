text```
Here's a complete CI/CD pipeline for a Java app connecting to RDS MySQL, deployed to a public EC2 server.

Assumptions
Public EC2 server with SSH access (key pair)
RDS MySQL already running, reachable from the EC2 server's security group
Simple Spring Boot app (works the same for plain Maven/Gradle apps too)
Sample Java app structure
table```
.
├── pom.xml
├── src/main/java/com/example/demo/
│   ├── DemoApplication.java
│   └── HelloController.java
├── src/main/resources/application.properties
└── .github/workflows/deploy.yaml

   
