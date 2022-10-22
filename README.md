# E-commerce-Back-End

## Description       
This is an E-commerce Back End application made by Hiu Sum Jaime Yue.         
In this E-commerce Back End application application, it allows you to read, create, update and delete data of Category, Product or Tag.         
When you run this E-commerce Back End application, you can open the API GET, POST, PUT and DELETE routes 
of Category, Product or Tag.       

The technologies I used in this project are Express.js, Sequelize and MySQL.

Below are the links to the starter code repository, this repository and the video of demostration.          
Starter code from https://github.com/coding-boot-camp/fantastic-umbrella         
Github repository: https://github.com/HiuSumJaimeYue/E-commerce-Back-End           
Video of demonstration: https://youtu.be/LrFeAt_odgs

## Table of Contents               
-[Installation](#installation)          
-[Usage](#usage)          
-[License](#license)          
-[Contributing](#contributing)          
-[Tests](#tests)        
-[Questions](#questions)        

## Installation         
If you are setting the project up in your local computer, run "npm i" in your terminal after downloading the files. Then, set up your .env file, an example of .env file is in the Tests Section. Run "mysql -u root" in your terminal if you did not set up a password for mysql. If you set a password for mysql, type "mysql -u root -p " in your terminal and enter your password. After the terminal showed "mysql>", type "source db/schema.sql". After seeing "Query OK, ...", type "quit" to get out of mysql. Next, type "npm run seeds". Finally, type "npm start". After seeing "Now listening" in the terminal, open Insomnia and start your changes.                

## Usage    
You can read all the Categories, Products or Tags.                
You can read or change or delete a single Category, Product or Tag using the Id at the end of the route.           
An example of HTTP request URL for Category, Product or Tag is in the Tests Section, including an example for using the Id at the end of the route.                 
You can also create a new Category, Product or Tag.         
An example of JSON that you can put in the body for creating a new Category, Product or Tag is in the Tests Section.            

            
## License         
&copy; 2022 by Hiu Sum Jaime Yue       
         
## Contributing         
Hiu Sum Jaime Yue --  E-commerce-Back-End   

## Tests        
The following is an example of .env file.           
// DB_PASSWORD is the password you set for your mysql.          
DB_NAME='ecommerce_db'          
DB_USER='root'                  
DB_PASSWORD=''          

The following is an example of HTTP request URL for Category, Product or Tag respectively.              
Category:  http://localhost:3001/api/categories                  
Product: http://localhost:3001/api/products            
Tag: http://localhost:3001/api/tags                 

The following is an example of HTTP request URL for Category, Product or Tag using Id at the end of the route.          
http://localhost:3001/api/categories/5

The following is an example of JSON that you can put in the body for creating a new Category.               
`{
  "category_name": "Food"
}`

The following is an example of JSON that you can put in the body for creating a new Product.               
`{
	"product_name": "Ball",
  "price": 50.57,
	"stock": 742,
	"category_id": 4,
  "tagIds": [4,5]
}`

The following is an example of JSON that you can put in the body for creating a new Tag.               
`{
	"tag_name": "NewTag"
}`

## Questions         
If you have any questions about the project, 
the GitHub link and email address of the author are shown below.                   
GitHub: [GitHub](https://github.com/HiuSumJaimeYue) 
& Email: [hiusumjaimeyue@cmail.carleton.ca](mailto:hiusumjaimeyue@cmail.carleton.ca)
