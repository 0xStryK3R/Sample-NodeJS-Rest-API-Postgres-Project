## Sample NodeJS Rest-API Project Using Postgres DB | ![Visitor Count](https://visitor-badge.glitch.me/badge?page_id=0xStryK3R.Sample-NodeJS-Rest-API-Postgres-Project)

1. Setup the DB Database:
      ```sql
      CREATE DATABASE node_api;
      CREATE USER node_admin WITH ENCRYPTED PASSWORD 'node_pwd';
      GRANT ALL PRIVILEGES ON DATABASE node_api TO node_admin;
      ```
2. Create Table using below command (in PgAdmin4 or psql):
    ```sql
    CREATE TABLE countries (
        ID SERIAL PRIMARY KEY,
        name VARCHAR(50),
        capital VARCHAR(50)
    );
    ```
3. Insert some data into the newly created _`countries`_ table:
    > _**Note:**_ _You can use sample insert queries provided in below file:_   
    > [_<img src="https://raw.githubusercontent.com/FortAwesome/Font-Awesome/6.x/svgs/regular/file-lines.svg" width="15" height="15"> countries.txt_](/countries_sample_data.txt) 

4. Clone Git-Repo into Local Directory.
5. Update DB credentials in _`queries.js`_ file as per your own DB configuration.
6. Open Command Line in main directory of project.
7. Run below command inside project directory to install required packages:
      ```console
      npm install
      ```
8. Run the project:  
    ```console
    node .\index.js
    ```  
    Or if you have nodemon installed:  
    ```console
    nodemon
    ```  
    > _**Note:**_ _To install nodemon, you can run the follow command (option `-g` is to install it globally.) :_   
    > ```npm install -g nodemon```  

9. All Done!! [`Click Here`](http://localhost:3000/) to interact with your app. 


> _**Assumptions**: NodeJS and Postgres has been setup and running prior to starting with this project._


> _**References**: For Complete details, please refer [`API Engineer: Node | Python | Django | Postman | PostgreSQL`](https://www.udemy.com/course/api-engineer-node-python-django-postman-postgresql/learn/lecture/27436790#overview) - the source material for this Repo._

    
