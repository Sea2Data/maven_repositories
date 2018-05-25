# maven_repositories
Project for storing maven repositories.

Copy from .jar and .pom from local .m2-directory after successfull build to appropriate directory in this project. The project can then be referred in a maven pom file as a regular dependency.


POM Reference to repos:
<repository>
  <id>sea2data_maven_repos</id>
  <url>https://raw.githubusercontent.com/Sea2Data/maven_repositories/release/</url>
</repository>

Example dependency:		
<dependency>
	<groupId>no.imr.sea2data</groupId>
	<artifactId>Formats</artifactId>
	<version>1.0.0</version>
	<scope>test</scope>
</dependency>
		
		
Havent found out yet how to deliver snapshot artifacts, so use release ...