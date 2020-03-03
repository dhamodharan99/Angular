To execute the code, download the .zip file and open the source folder. And run the following commands on path, where you have the package.json and db.json.
1. npm install,
2. npm install bootstrap@4 jquery --save
3. npm install -g json-server
4. Run 
json-server --watch db.json
5. And open the code on Visual studio code editor. And do the "ng serve --open" on the  New Terminal.
-----------------------------------------------------------------------------------------------------------------------------------------------------------

Other Details:
I. REST with Reactive form, Rxjs, Get, Put And Post On fake Json-server, Cross field validation, Custom validations:

Steps:
1. Install Node and NPM using the link :  https://nodejs.org/en/download/
2. node -v
3. npm -v
4. npm install -g @angular/cli
5. npm install -g @angular/cli@latest
6. https://code.visualstudio.com/download
7. ng new Angular6Project
8. cd Angular6Project
9. npm install bootstrap@4 jquery --save

10. Modify angular.json :
"styles": [
  "src/styles.css",
  "node_modules/bootstrap/dist/css/bootstrap.min.css"
]
"scripts": [
  "node_modules/jquery/dist/jquery.min.js",
  "node_modules/bootstrap/dist/js/bootstrap.min.js"
]

11. A quick additional test to verify, Bootstrap styles work as expected, include the following button in the root component (app.component.html) file.
<button class="btn btn-primary">
    Bootstrap Styled Button
</button>

12.
ng g c employee/create-employee --flat=true 
ng g c employee/list-employees --flat=true
ng generate service employee -module=app.module --flat=true

13. Execute the following NPM command to install JSON server
npm install -g json-server 

14. 	Create db.json file in the root project folder. Copy and paste the following JSON data in the file.
{
    "employees": [
        {
            "id": 1,
            "fullName": "Mark",
            "contactPreference": "email",
            "email": "mark@email.com",
            "phone": "5641238971",
            "skills": [
                {
                    "skillName": "C#",
                    "experienceInYears": 1,
                    "proficiency": "beginner"
                },
                {
                    "skillName": "Java",
                    "experienceInYears": 2,
                    "proficiency": "intermediate"
                }
            ]
        },
        {
            "id": 2,
            "fullName": "John",
            "contactPreference": "phone",
            "email": "john@email.com",
            "phone": "3242138971",
            "skills": [
                {
                    "skillName": "Angular",
                    "experienceInYears": 2,
                    "proficiency": "beginner"
                },
                {
                    "skillName": "HTML",
                    "experienceInYears": 2,
                    "proficiency": "intermediate"
                },
                {
                    "skillName": "LINQ",
                    "experienceInYears": 3,
                    "proficiency": "advanced"
                }
            ]
        }
    ]
}

15.  Execute the following command to start the server
json-server --watch db.json
Run npm i -g json-server to update
 
---------------------------------------------------------------------------------------------------------------------------------------------------------

II. Angular custom preloading strategy with REST, Reactive form, Rxjs, Get, Put And Post On fake Json-server, Cross field validation, Custom validations:
Steps:
1. Install Node and NPM using the link :  https://nodejs.org/en/download/

2. node -v

3. npm -v

4. npm install -g @angular/cli

5. npm install -g @angular/cli@latest

6. https://code.visualstudio.com/download

7. ng new Angular6Project

8. cd Angular6Project

9. npm install bootstrap@3 jquery --save

10. Modify angular.json :
"styles": [
  "src/styles.css",
  "node_modules/bootstrap/dist/css/bootstrap.min.css"
]
"scripts": [
  "node_modules/jquery/dist/jquery.min.js",
  "node_modules/bootstrap/dist/js/bootstrap.min.js"
]

11. A quick additional test to verify, Bootstrap styles work as expected, include the following button in the root component (app.component.html) file.
<button class="btn btn-primary">
    Bootstrap Styled Button
</button>

12.
ng g c employee/create-employee --flat=true 
ng g c employee/list-employees --flat=true

To create this new Employee feature module. Here is the command.
ng g m employee/employee --flat -m app

Use the following to generate a SharedModule
ng g m shared/shared --flat -m employee/employee

To generate the service, use the following Angular CLI command
ng g s CustomPreloading

Use to create the HomeComponent
ng g c home --flat

Use to create the PageNotFoundComponent
ng g c page-not-found --flat

13. Execute the following NPM command to install JSON server
npm install -g json-server 

14. 	Create db.json file in the root project folder. Copy and paste the following JSON data in the file.
{
    "employees": [
        {
            "id": 1,
            "fullName": "Mark",
            "contactPreference": "email",
            "email": "mark@email.com",
            "phone": "5641238971",
            "skills": [
                {
                    "skillName": "C#",
                    "experienceInYears": 1,
                    "proficiency": "beginner"
                },
                {
                    "skillName": "Java",
                    "experienceInYears": 2,
                    "proficiency": "intermediate"
                }
            ]
        },
        {
            "id": 2,
            "fullName": "John",
            "contactPreference": "phone",
            "email": "john@email.com",
            "phone": "3242138971",
            "skills": [
                {
                    "skillName": "Angular",
                    "experienceInYears": 2,
                    "proficiency": "beginner"
                },
                {
                    "skillName": "HTML",
                    "experienceInYears": 2,
                    "proficiency": "intermediate"
                },
                {
                    "skillName": "LINQ",
                    "experienceInYears": 3,
                    "proficiency": "advanced"
                }
            ]
        }
    ]
}

15.  Execute the following command to start the server
json-server --watch db.json
---------------------------------------------------------------------------------------------------------------------------------------
