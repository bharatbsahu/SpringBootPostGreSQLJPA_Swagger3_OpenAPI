------------------------------------- Step To Implement Swagger2 ---------------------------------------
1) Add this dependency in pom.xml:

		<dependency>
			<groupId>io.springfox</groupId>
			<artifactId>springfox-swagger-ui</artifactId>
			<version>3.0.0</version>
		</dependency>
		<dependency>
			<groupId>org.springdoc</groupId>
			<artifactId>springdoc-openapi-ui</artifactId>
			<version>1.6.9</version>
		</dependency>
		<dependency>
			<groupId>io.springfox</groupId>
			<artifactId>springfox-swagger2</artifactId>
			<version>2.9.2</version>
		</dependency>
		
		Incase Plugin Error, Add this depen :
		
		<dependency>
            <groupId>org.springframework.plugin</groupId>
            <artifactId>spring-plugin-core</artifactId>
            <version>2.0.0.RELEASE</version>
        </dependency>
		
2) "@Tag" Annotation in RestController Main Class

	import io.swagger.v3.oas.annotations.tags.Tag;
	
	@RestController
	@Tag(name = "Employee Details Specification", description = "Employee Details")

3)	Add this Annotanion "@ApiOperation" 

	import io.swagger.annotations.ApiOperation;

	@GetMapping("/employees")
    @ApiOperation(value = "Return All the Employee Details")
	
4) Swagger2 URL -> http://localhost:8080/swagger-ui/index.html

	http://localhost:8080/employees
	
	Git -> https://github.com/bharatbsahu/SpringBootPostGreSQLJPA_Swagger2
	
