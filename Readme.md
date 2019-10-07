## Spring Boot RestFul API With Swagger API Docs integration for ClockFour Assessemnt Solution
## Steps to Setup

**1. Clone the repository** 

https://github.com/suyeshsiroya/multi-data-techniques-service.git


**2. Specify all the image uploads/output directory & file names**

Open `src/main/resources/application.properties` file and change the below properties 
## Image File Storage Properties
image.folder=C:/Softwares/uploads
# If an image already exists in image.folder, move to below configured archive folder
archive.folder=C:/Softwares/archive
# Output the 3 columns of employee list (pipe delimited) into below output file location (output.folder, output.file)
# if folder is kept empty then file will  be saved in project executable directory
# output folder is used as folder for output excel file as well.
# complete output file location will be "output.folder/output.file"
output.folder=C:/Softwares/outputs
output.file=employee_output.txt
#Parsed XML elements of Employee lists to be written into below excel file name
# complete excel file location will be "output.folder/xls.name"
xls.name=employees_sheet.xlsx


**3. Run the app using maven**

```bash
cd 
mvn spring-boot:run
```

That's it! The application can be accessed at `http://localhost:8080`.

.war is already included in the solution that can be run on tomcat server.
You may also package the application in the form of a jar by changing th the pom.xml and then run the jar file like so -

```bash
mvn clean package
java -jar target/multi-data-techniques-service-0.0.1-SNAPSHOT.jar
```
