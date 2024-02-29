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

# Properties file
@PropertySource("abc.properties")  --> loading random properties file to spring.

# to run the jar file not present in fat jar
java -jar abc.jar --spring.config.location=/def/ghy/xxx/a.properties  --> to use th poperties file run time

# spring life cycle hooks annotations.
@PostConstruct  --> initilizing anything or execute anyting after bean creation in the container by dispatcher servlet.
@PreDestroy --> execute anyting just before bean deletion in the container (when container also being closed) by dispatcher servlet.

# spring boot autoconfiguration
Autoconfiguration file which has list of all autoconfiguration classes.
if you mark the spring application with @EnableAutoConfiguration, it reads the file and create the objects.
spring boot uses intelligence, it does not create object which you do not require.
it uses annotation @ConditionalOnclass(Servlet.class), to check if maven dependency added/servlet class file added to the dependency or not, the only it creates object in the autoconfigure process, otherwise it wont create.

