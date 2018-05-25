# maven_repositories
Project for storing maven repositories.

Copy from .jar and .pom from local .m2-directory after successfull build to appropriate directory in this project. The project can then be referred in a maven pom file as a regular dependency.


POM Reference to repos:
<code>

&lt;repository&gt;

  &lt;id&gt;sea2data_maven_repos&lt;/id&gt;
  
  &lt;url&gt;https://raw.githubusercontent.com/Sea2Data/maven_repositories/release/ &lt;url&gt;
  
&lt;/repository&gt;

</code>

Example dependency:		

<code>
&lt;dependency&gt;

	&lt;groupId&gt;no.imr.sea2data&lt;/groupId&gt;
	
	&lt;artifactId&gt;Formats&lt;/artifactId&gt;
	
	&lt;version&gt;1.0.0&lt;/version&gt;
	
	&lt;scope&gt;test&lt;/scope&gt;
	
&lt;/dependency&gt;

</code>
		
		
Havent found out yet how to deliver snapshot artifacts, so use release ...