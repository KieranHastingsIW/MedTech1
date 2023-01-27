# MedTech1
basic med tech microservice that adds info to a database and calls RL API when connected 

* Ensure that Docker desktop is running if you are working from a windows machine.
* Run `docker-compose -f medtech-compose.yml up --build -d` to build the med tech application and db
* Run `docker-compose -f record-compose.yml up --build -d` to build the record locator application and db
* When both compose files have built successfully open your search engine of choice and lookup `localhost:8080/mdtech this will take you to a forms page with text boxes to input patient information 
* Enter in patient information and click submit 
* A webpage should return with the statement "Patient submitted successfully" and the patients NHI number

* To Test to see if the record has successfully been recorded in the record locator database in Postman import the  rl-test.json file and run the Get request with the NHI number you submitted to the medtech web form.
* The output should be a 200 OK status and an array of Record Locator objects showing the recordLocatorId systemId, dataType, and the patientId which will be equivilant to the NHI.


