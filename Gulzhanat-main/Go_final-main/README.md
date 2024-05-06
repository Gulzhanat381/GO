# Final Project Description: University Canteen Management System Documination
Below are the steps to launch the application on your device:
* Download the repository
* Create a database locally to run the application (database name = go_db user=postgres password = 123,
if your local database is different, change the values ​​accordingly in the database.go file in the Init() function)
* Create tables in the database as in the init.sql file
* run the code using the command "go run main.go" (you need to have the go compiler installed on your system)
* Done, the application runs on port 8080

Below are the steps to run an application in Docker:
* Download the repository
* Open the console, type “docker-compose up --build” (You need to have Docker on your system)
* Done, the application runs on port 8080

If you need to add an admin user to the database when working with Docker, follow these steps:
* Add a user to the database via api (By default, all registered users have the role "user")
* Open CMD
* Register docker ps
* In the list of containers, find postgres
* docker exec -it <postgres_container_name> bash
* Write the command "psql -h localhost -U postgres -W"
* Enter the password "123"
* Enter the command "\c go_db"
* You are now in the db_go database and can assign administrators

Technologies used:
Golang
Gin framework
Postgresql
Docker

Libraries used:
github.com/dgrijalva/jwt-go (creating JWT tokens)
golang.org/x/crypto (encrypt user passwords)


If you have any additional questions, write to Telegram: @ggulzhanat03
-- 
