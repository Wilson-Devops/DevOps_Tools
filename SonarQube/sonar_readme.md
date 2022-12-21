# SonarQube
SonarQube is an open-source platform developed by SonarSource for continuous inspection of code quality to perform automatic reviews with static analysis of code to detect bugs and code smells on 29 programming languages


-   STEP-1  -   Launch a SonarQube Virtual Machine/Instance or Contanarise or SAAS
-   STEP-2  -   Login to SonarQube
-   STEP-3  -   Create a project in SonarQube
    -   Organisation Name:
    -   Type of Project:
    -   Project URL:
    -   Project Key:
-  STEP-4   -   Take the above details and integrate with SCM/VCS i.e Source Code pom.xml
-  STEP-5   -   Create a code build job in AWS & Execute Sonar Goal
   -  #mvn verify sonar:sonar
- STEP-6    -   Validate & Clean Up!


#### SonarQube Integration
-   Login to SonarQube
-   Click on + symbol and click on Analyze projects
-   Select create a project manually   
    
    - Organization : manda-sonar 
    - Project key : awsdevopssonar-codescan
    - Display name : awsdevopssonar-codescan
    - Project visibility : Public
    - Click on Create
    - Select Configure and click on Manually 
    - Click On Maven
          
          - Configure the SONAR_TOKEN environment variable
          - Name of the environment variable: SONAR_TOKEN
          - Value of the environment variable: 9adc3c86c767fe01191e7d86c11991bf5c932e7f
          - Execute the SonarScanner for Maven from your computer Update your pom.xml file with the following properties: 
          - 