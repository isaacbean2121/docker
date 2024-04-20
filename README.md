Challenge 3.

First, I had to create a new project because the github link was broken for me. After That I created docker-compose.yml file with the help of A.I, along with this video: 24GCD001Q GenAI Performance v12 (youtube.com). This video also helped me figure out that before running docker-compose ps, you must build the container using docker-compose up --build -d. I had to modify the docker file slightly to replace this line COPY docker/api/package*.json ./
With this line: COPY package*.json ./. I followed one of the videos provided by the assignment to create the env file, which went smoothly. 


Challenge 4: 

I quickly found the command to use after browsing the docker documentation. Use Docker Compose | Docker Docs. I used the command, > docker-compose up --scale node-service=3 -d, right away but got an error that led me to comment out a line in my docker.compose.yml file.


After that I had to rebuild using these commands: PS C:\Users\isaac\Downloads\challenge3 (2)> docker-compose down
>> docker-compose up --build -d
>> docker-compose up --scale node-service=3 -d






