# MedTech1
basic med tech microservice that adds info to a database and calls RL API when connected 

* Run `docker-compose up --build` to build the med tech application and db
* Search for localhot:8080/medtech this should take you to a forms page with text boxes to input patient information 
* Enter in patient information and click submit 
* a webpage should return with the statement "Patient submitted successfully" and the patients NHI number
* When this micro service is connected with the RL microservice this NHI, the Systems credentials and the datatype will be passed to the record locator and stored there, currently this method is commented out and replaced by a print statement.
* The print statements reads "this is the call that is made when posting to the record locator" and can be seen in the terminal from the container labelled medtech 
