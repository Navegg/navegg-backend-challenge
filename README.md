# Navegg Back-end Challenge - Create an API

The general purpose is receiving a list of websites, and organize this information to classify and store all the details of the website.  

## Briefing  
The application must import a CSV file and add it to a database. This CSV contains some sites with their URLs and categories. You must develop an API to make a CRUD of these sites after import.


## Project requirements
- The project needs to be written in Python, Ruby, Java, GoLang or similar (with framework or not);
- The code (including the variables names and comments) must be in English;
- The project needs documentation that anyone can install and test your application only by reading it;

### The application needs to have the following features:
- Import a CSV file [from here](https://raw.githubusercontent.com/Navegg/navegg-backend-challenge/master/sites.csv) and add in a database (you must modeling a database according to data in the CSV file).
- A REST API for CRUD.

### At a minimum, this must:
- Planning a relational database based on the relation of the field in the database;
- Ensure that register exists before delete or update;
- Avoid duplicated site names;
 
### Bonus points for:
- We use Django Rest Framework internally, so using this framework in your application is a plus.


### What we are going to evaluate:
- Code abstraction! Reusable functions are better than hard code;
- Less code is better! If you can do the application with a little as possible of code, it’s a plus;
- Clean code! We need to read and understand what you’ve done;
- Documentation! Simple documentation that explains the main points.

## Technical specifications 

### The CSV has the following columns:
| Colum  | detail |
| -- | -- |
| name | The site name |
| URL | The page URLs (semicolon separated)
| category | The page categories (semicolon separated)
| status | The page status

#### Important:
- The page entity can take N URLs and N categories.


### API endpoints:
    GET:    /item/ -> list all active register in the database.
    GET:    /item/[id]/ -> list one register.
    POST:   /item/ -> create new register.
    PATCH:  /item/[id]/ -> modify register
    DELETE: /item/[id]/ -> remove register


## To conclude
Please submit your solution as a pull request to this repository or email a zip directly to challenge@navegg.com, and include in it:
- The source code;
- A link to your API working properly (or instructions to run locally);
- How long it took for you to get it done;
- What you would add/change if you had more time
    
Thanks, and have fun!
