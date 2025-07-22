# User Guide : How to Install and setup JSON server

### Author : *Sylvia*
### Date : *July 2025*

## INTRODUCTION:
JSON Server is a tool that helps to simulate all types of HTTP requests (GET,PUT,POST,DELETE). It allows users to create a mock rest API quickly using a simple JSON file. It is mainly used by front-end developers and testers for data transfer using the above HTTP methods. 
This guide explains how to install and set up JSON Server on your local machine. 
PREREQUISITES:
- Install ``node JS ``
- Use this link for the download [https://nodejs.org/en](https://nodejs.org/en)
- Open terminal/command prompt to check whether node JS is present. Use the command, npm -version
## INSTALLATION:
STEP 1: Open terminal/command prompt
STEP 2: Give the command, ``npm install -g json-server``
(Note: JSON Server will be installed globally so that you can run it from anywhere on your system)
## CREATE A JSON FILE:
Create a JSON File with name db.json. This will act as your database.
Sample JSON file,
```
{
  "employees": [
    {
      "id": "1",
      "first_name": "abc",
      "last_name": "xyz",
      "email": "abcxyz@gmail.com"
    },
    {
      "id": "2",
      "first_name": "def",
      "last_name": "ghi",
      "email": "defghi@gmail.com"
    }
]
}
```
## RUNNING THE SERVER:
Once you have created your db.json file, you need to run the server.
Open your terminal/command prompt and run,
``json-server - -watch db.json ``
This command will run the server and watch for changes in db.json file. By default, the server will be hosted at `` http://localhost:3000/employees `` and you can start making HTTP requests to the endpoints defined in the JSON file. 
Open a browser to see your mock api in action.
TESTING ENDPOINTS:
You can test this api in tools like POSTMAN. For example,
**GET** http://localhost:3000/employees 
You will get the list of all the employees in the JSON format.
CONCLUSION:
You have successfully installed and set up your JSON Server. You can now create and test APIs with your data. 


