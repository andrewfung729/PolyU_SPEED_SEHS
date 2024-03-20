# 2. Development Environment Configuration - IntelliJ IDEA Ultimate Edition

## Java Development Kit (JDK)

JDK Path

```bash
/Library/Java/JavaVirtualMachines/openjdk.jdk/Contents/Home
```

## Java Servlet Container

> For Tomcat 9, select Java EE 8. For Tomcat 10, select Jakarta EE 9.1.

### Apache Tomcat

#### Add tomcat

Tomcat base directory:

```Bash
/opt/homebrew/opt/tomcat/libexec
```

#### Edit URL

1. Edit Configuration → Deployment
    - 如果你Set Application context係咁: `/test_java`
    - URL就會係咁: `http://localhost:8080/test_java/`
   > ❗❗❗ 經同學反映，冇行到佢跟畀你嘅commands，會產生大麻煩，請不要忘記！
   TomEE 用呢個URL會唔得，要用返個folder名: XXX-1.0-SNAPSHOT

2. Hot Swap
    - Choose war exploded
    - On ‘Update’ action: Redeploy (Press ⌘Сmd + F10)
    - On frame deactivation: Update classes and resources
    - [https://www.jetbrains.com/help/idea/updating-applications-on-application-servers.html](https://www.jetbrains.com/help/idea/updating-applications-on-application-servers.html)

### Apache TomEE

TomEE base directory:

```bash
/opt/homebrew/opt/tomee-plus/libexec
/opt/homebrew/opt/tomee-plume/libexec
```

## J2EE Servlet Template (Optional) {collapsible="true"}

為Servlet創建一個模板，以便在IntelliJ IDEA中快速生成Servlet文件。

- [https://www.jetbrains.com/help/idea/creating-and-configuring-web-application-elements.html](https://www.jetbrains.com/help/idea/creating-and-configuring-web-application-elements.html)

```Java
#if (${PACKAGE_NAME} && ${PACKAGE_NAME} != "")package ${PACKAGE_NAME};#end
#parse("File Header.java")

import jakarta.servlet.*;
import jakarta.servlet.http.*;
import jakarta.servlet.annotation.*;
import java.io.IOException;

@WebServlet(name = "${Class_Name}", value = "/${Class_Name}")
public class ${Class_Name} extends HttpServlet {

    /**
     * @see HttpServlet#HttpServlet() 
     */ 
    public ${Class_Name}() { 
        super(); 
     } 
      
    /**
     * @see Servlet#init(ServletConfig)
     */
    @Override
    public void init(ServletConfig config) throws ServletException {

    }

    /**
     * @see HttpServlet#doGet(HttpServletRequest, HttpServletResponse)
     */
    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {

    }

    /**
     * @see HttpServlet#doPost(HttpServletRequest, HttpServletResponse)
     */
    @Override
    protected void doPost(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {

    }

    /**
     * @see HttpServlet#doPut(HttpServletRequest, HttpServletResponse)
     */
    @Override
    protected void doPut(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {

    }

    /**
     * @see HttpServlet#doDelete(HttpServletRequest, HttpServletResponse)
     */
    @Override
    protected void doDelete(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {

    }

    /**
     * @see Servlet#destroy()
     */
    @Override
    public void destroy() {

    }
}
```

## Plugins

- Jakarta EE: Enterprise Java Beans (EJB)

## Issues

- [https://blog.csdn.net/qq_29259155/article/details/81410184](https://blog.csdn.net/qq_29259155/article/details/81410184)

## References

- [https://www.jetbrains.com/help/idea/creating-and-running-your-first-java-ee-application.html](https://www.jetbrains.com/help/idea/creating-and-running-your-first-java-ee-application.html)
- [https://blog.csdn.net/J080624/article/details/80070597](https://blog.csdn.net/J080624/article/details/80070597)
- [https://blog.csdn.net/wangpaiblog/article/details/114156312](https://blog.csdn.net/wangpaiblog/article/details/114156312)
