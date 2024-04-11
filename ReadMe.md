# Day 3

## Web Application with SpringBoot

@ResponseBody-
• The **`@ResponseBody`** annotation informs a controller that the object returned should be **serialized into JSON** and included in the HTTP response.

Note that if a controller is annotated with **`@RestController`**, Spring automatically applies **`@ResponseBody`** by default.

```
@Controller
public class SayHelloController {

    @RequestMapping("say-hello")
    @ResponseBody
    public String sayHello(){
        return "Hello! What are you learning today?";
    }
}
```

For intelliJ the dependency for TomCat jasper is 

```
<dependency>
   <groupId>org.apache.tomcat.embed</groupId>
   <artifactId>tomcat-embed-jasper</artifactId>
</dependency>
```

And for eclipse

<dependency>
	<groupId>org.apache.tomcat.embed</groupId>
	<artifactId>tomcat-embed-jasper</artifactId>
	<scope>provided</scope>
</dependency>
