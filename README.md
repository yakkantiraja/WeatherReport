WeatherReport
=============

To get weather details
Installation

1) Unzip the WeatherReport.zip file
2) Open Eclipse
3) Goto File/Import
4) Click on  Existing project into workspace
5) Browse folder location
6) Select extracted folder(WeatherReport)
7) Click finish

Note :
Eclipse should precofigured with maven

In case of commpilation problem , please do the below steps
1)RightClick on the project
2) Goto Maven ---> Update project
3) For java.lang.ClassNotFoundException: org.springframework.web.context.ContextLoaderListener
	properties ---> Deployment Assembly -- Add --java Build path Entries -- Maven Dependencies

To Build war
1) RightClick on the project 
2) Run As --> Maven install
3) it will create the WeatherReport.war file in target folder

To Run in Eclipse

1) RightClick on the project
2) Run As --> Run on Server -- Select the server -- Finish
3) Browser will open the application with
 url http://localhost:{portno}/WeatherReport/search

 To Test 

 1) Open Applcaition 
 2) click on submit with out entering zipcide
      --Invalid ZipCode Code Format message will appear
3) Enter any  random no more than 6 characters
	--Invalid ZipCode Code Format message will appear
4) Enter valid zipcode(12345)
	-- Will display the City name,State and temprature both in F & C

