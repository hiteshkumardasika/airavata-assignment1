# airavata-assignment1
The project contains three micro services written in Java,Python and Go respectively.
Pre-requisite

Install go

Install Java

Install Docker


docker run --name mysql-cont -p 3306:3306 -e MYSQL_ROOT_PASSWORD=root -d mysql:5.5

Micro-Service One: JAVA

The Microservice is a spring application. It is located in microservice_one directory.

docker run -it -p 5484:8080 --name app_new --link mysql-cont:db msone

Micro-service Two: Python

This microservice is a flask-mysql application. It is located in microservice_two directory.
docker run -it -p 5001:5000 --name app_2 --link mysql-cont:db ms2

Micro-service Three: Go 

This microservice is in go language. It is located in microservice_three directory

cd microservice_three

go build

execute the binary generated.



Accessing the UI
Open Index.html. It has links to register and login. First register yourself.

It redirects to login page and remember the username and password used for registration and enter here.

Now you see the todo list box to add your todo.

