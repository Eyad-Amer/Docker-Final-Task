# Docker Final Task
![image](https://user-images.githubusercontent.com/40535130/202915030-5ddbe91f-8a27-4161-80e7-29cad2f23b2b.jpg)


###  About 

------------

#####  1- Create a Python Web APP (use either Flask or FastAPI libraries) that:
##### ● Presents the Current BitCoin Price
##### ● Stores the price in a Redis Database
##### ● Presents the Average Price for the last 10 minutes
##### 2- Dockerize the applications (Create Dockerfile and docker-compose.yml)
##### 3- Create a Jenkinsfile for CI/CD that creates and pushes the generated Web application Docker image to Docker Hub

### Steps To Running The web Application:

------------

#### Clone The Project:
	git clone https://github.com/Eyad-Amer/Docker-Final-Task.git
#### Build The Project:
	docker compose up
![docker compose up](https://user-images.githubusercontent.com/40535130/202915243-e415a7b0-2c70-4754-8cc7-b7712a2502c6.jpg)


#### Run The Project:
	http://localhost:8000/
note: to present the Average Price for the last 10 minutes, you need to wait 10 mins when running the localhost
![browser app](https://user-images.githubusercontent.com/40535130/202915136-e41aac8b-cd54-479a-9d21-17029bdc2fcf.jpg)

####  Stop The Project:
	docker compose down
![docker compose down](https://user-images.githubusercontent.com/40535130/202915306-2075dbcc-02d7-4a16-b2cd-5bc7b8ecc2b1.jpg)

### Jenkins Stage View

------------

![jop](https://user-images.githubusercontent.com/40535130/202915370-aaaf9243-6343-4702-9ef0-d22a5df89552.jpg)

### DockerHub

------------

![dockerHub](https://user-images.githubusercontent.com/40535130/202915421-843e826c-6777-4c0d-b9f3-fc4f0d322124.jpg)


