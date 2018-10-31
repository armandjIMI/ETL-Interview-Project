# ETL-Interview-Project
Greetings Candidate!! Thank you for taking the time to complete the side project. This project aims to simulate a small portion of the system you may be developing on. Here we aim to test test technical proficiency and understanding of the tech stack.

We are looking forward to have a chat with you after reviewing your work. Good luck!

## Scenario
Build a RESTFull API which has the following features:

- Create, Read, Update and Delete a client configuration
- Collect a data file from a preconfigured directory
- Extract the data from the collected file
- Apply some validation on the collected data
- Write valid/invalid data to a preconfigured output directory

## Business Rules
- A client has a Name
- A ftpcollection has a name, path, file type
- File types supported for both input: comma delimited csv, pipe delimited csv and json
- The output file type is json
- File structure to expect: First name, last name, product code, RSA ID Number and (cellnumber or email address)
- The file output needs to be split on valid/invalid email addresses and cellnumber
- A file can contain either a  cellnumber or email address (bonus points if the API can handle both columns in the same file)
- Output directory with the following naming convention: [YYYYMMDDHH] all files processed needs to be written out to the corresponding directory
- Output file's naming conventions: [clientname]_[origionalfilename]_[indicator (cellnumber/email)]_[valid/invalid]_[YYYYMMDDHH].json

## Tech Stack
- C#
- .Net Framework or .NET Core
- MS-SQL
- EntityFramework or EntitiyFramework Core or any other mirco ORM (bonus points if you're hard core enough to do classic ADO.NET)
- Swagger for API documentation
- Your choice of logging software (I'd recommend serilog for .net core project or log4net for .Net framework project)

> Note: A front end is not required for this project however should you have time to attend to it then either a MVC or Vuejs
> Note: All configuration settings must be moved out to a config file either the  or appconfig
> Bonus: Build a validation API which handles the RSA ID Number, Cellnumber and email validation

## Design Patterns
ensure the project implement the following patterns:
- Some level of Domain Driven Design
- Factory pattern

## Design Principles
Ensure the code is guided by the below patterns:
- SOLID
- Separation of concern
- Repository pattern is optional but not required as we are not building a huge repository layer for this project

## Review
- You can either fork this repo or create your on your Github profile and send us the link when you are done
- We will also review your public github projects should they be available
- Please ensure that you complete a detailed readme.md containing all relevant commands to run the api on a new machine
