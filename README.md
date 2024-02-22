# springbootlearn
@ComponentScan
@EnableAutoConfiguration --> able to start the application in tomcat/starts the tomcat -> ServletWebServerFactory
Spring WebServerApplicationContext(I) is the container for web application.
@Bean -> Manually creating the bean and pushing into the container.
@Configuration -> this is a configuration file that holds bean defination.
@SpringBootConfiguration -> this is same as @configuration , this marker annotation, which holds beans defination.

# The building block of Spring boot application is 
@EnableAutoConfiguration
@ComponentScan
@SpringBootConfiguration

@SpringBootApplication --> same as above, all the 3 annotations are present in this annotation.

