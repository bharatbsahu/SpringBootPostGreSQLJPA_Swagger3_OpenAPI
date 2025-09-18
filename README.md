------------------------------------- Step To Implement Swagger Open API 3 ---------------------------------------
1) Add this dependency in pom.xml:

		<dependency>
		    <groupId>org.springdoc</groupId>
		    <artifactId>springdoc-openapi-starter-webmvc-ui</artifactId>
		    <version>2.8.13</version>
		</dependency>
		
		<dependency>
		    <groupId>io.swagger</groupId>
		    <artifactId>swagger-annotations</artifactId>
		    <version>1.6.16</version>
		</dependency>
		
2) "@Tag" Annotation in RestController Main Class

	import io.swagger.v3.oas.annotations.tags.Tag;
	
	@RestController
	@Tag(name = "Employee Details Specification", description = "Employee Details")

4) Swagger2 URL -> http://localhost:8080/swagger-ui/index.html
	http://localhost:8080/employees
	
	Git -> https://github.com/bharatbsahu/SpringBootPostGreSQLJPA_Swagger3_OpenAPI

http://localhost:8080/v3/api-docs
http://localhost:8080/swagger-ui.html

