# Java Application 

# Spring Boot + JSP Setup

This project uses Spring Boot as the backend and JSP as the frontend.  
JSP pages are rendered from the server using Spring MVC.

---

## 📌 Requirements
- Java 17+
- Maven
- Spring Boot (Web, Tomcat, Thymeleaf removed)
- JSP engine support
- MySQL or H2 (Optional)

---

## 📂 Folder Structure

src/main/
 ├── java/com/example/
 │      ├── controller
 │      ├── service
 │      ├── repository
 │      └── model
 └── resources/
       ├── static/
       ├── templates/ (Not used)
       └── application.properties

src/main/webapp/
 └── WEB-INF/views/
       ├── home.jsp
       └── login.jsp

---

## ⚙️ Add Dependencies (pom.xml)

```css
<dependency> <groupId>org.apache.tomcat.embed</groupId> <artifactId>tomcat-embed-jasper</artifactId> </dependency> <dependency> <groupId>javax.servlet</groupId> <artifactId>jstl</artifactId> </dependency> 
```
## application.properties
```css
spring.mvc.view.prefix=/WEB-INF/views/
spring.mvc.view.suffix=.jsp
server.port=8080
```



