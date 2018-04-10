# Spring Boot Sample One Project 


1. Create account on GitHub.
    
2. Open https://github.com/krprashantjha/DigitalEx
    
3. First fork, then clone the URL
    
4. Import that URL in eclipse. Follow below project and make change.
    
5. Once change is completed. Then commit with proper message and push the project.
    
6. You will see that project in your local of GitHub site.
    
7. Place Pull Request and inform the owner of the repository.


# Please Follow all steps carefully

1.	Import the project and run maven install

2.	Run the application as Spring boot

3.	Look for the swagger documentation http://localhost:8080/index.html

4.	This has a Account REST resource which has findAllAccounts() API

5.	FindAllAccounts returns the account provided in a static list with account name as Account1, Account2 and Account3.

6.	Implement the getAccount 

    a)	Returns the Account object for a given accountId with status as success. 

    b)	If account does not exist then return 404 with custom error with message and error code e.g. {"errorMessage": "Account with       id 123 not found", "errorCode": "NOT_FOUND" }

7.	Implement createAccount 

    a)	Adds the account in the static list and returns 201 if success. 

    b)	If account with that name already exists then RETURN HTTP error code 409(CONFLICTED) with a custom message "Unable to   create. A  Account with name already exist"

8.	Include the swagger docs for both getAccount and createAccount

9.	Add another resource "UserResource" with APIs getUsers and createUser. This returns users associated for an given account id    and saves the user under an account.

10.	Enable the Retry mechanism on account resource if there is 404 error while retrieving the getAccount by a given id.
