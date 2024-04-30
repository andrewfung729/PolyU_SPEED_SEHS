# SEHS4701 SpringBoot Development Environment Configuration - IntelliJ IDEA Ultimate Edition

1. Open the existing project folder in IntelliJ IDEA
    - Click Open
      ![idea-open-folder.png](idea-open-folder.png)
2. Open the Run/Debug Configurations dialog
    - Click the dropdown menu next to the Run button
    - Click Edit Configurations...
      ![idea-open-run-config.png](idea-open-run-config.png)
3. Add a new Spring Boot configuration
    - Click the + button
    - Select Spring Boot
      ![idea-run-config-add-springboot.png](idea-run-config-add-springboot.png)
4. Configure the Spring Boot configuration
    - Name: SpringBoot
    - Java: 21
    - Main class: choose the main class of your Spring Boot application
      ![idea-run-config-springboot-config.png](idea-run-config-springboot-config.png)
5. Import the Maven project
    - Click the Lifecycle tab
    - Right-click on the `install` goal
    - Click Run 'Run Maven Build'
    - ![idea-maven-install.png](idea-maven-install.png)
6. Compile the Spring Boot by Maven
    - Click the Lifecycle tab
    - Right-click on the `compile` goal
    - Click Run 'Run Maven Build'
    - ![idea-maven-compile](idea-maven-compile.png)
7. Run the Spring Boot application
    - Click the Run button
      ![idea-run-springboot.png](idea-run-springboot.png)