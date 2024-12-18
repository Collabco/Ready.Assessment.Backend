# Serverless API Demo Project assessment

## Summary
This is a basic project that includes a lot of the areas that you wold be expected to do in your day to day role.

<B>There is no way you will complete most of this by the time your technical test, but it should
give you a chance to demostrate your technical skills.</b>

## Requirements
1. Write a Create Student Http Azure function using the appropriate method and returning appropriate status code with a uniquely generated id.  This should accept a StudentInputModel with properties mentioned below.  The model should be validated and added to service bus for adding to datastore later.
2. Create a Process Student Event Service Bus Azure Function that listens to Service bus populated in part 1 and adds the Student to a Data Model.
3. Create 1 or more Unit Tests in dedicated project to demonstrate that the Azure Function works as designed.
4. Write a Edit Student Http Azure function using the appropriate method and returning appropriate status code.  This should accept a StudentInputModel with properties mentioned below.  The model should be validated and added to service bus for updating in the datastore later.
5. Write a Delete Student Http Azure function using the appropriate method and returning appropriate status code.  This should accept a StudentInputModel with properties mentioned below.  The model should be validated and added to service bus for deleting from datastore later. 
6. Finish setting up pipeline file to build and deploy the Azure Functions project to the cloud.

## Supporting Information
You will need to create a StudentInputModel Class, with following properties.
UPN string mandatory
FirstName string mandatory
LastName string mandatory
OtherNames string
DateOfBirth DateTime Between 01/01/1900 and 31/12/2008

Return Success Code for  completed requests.
Return appropriate Code for validation errors and / or expected error conditions.

