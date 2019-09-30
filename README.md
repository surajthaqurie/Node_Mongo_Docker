### Introduction
- This Project is just of implementing Docker in Node app.

#### Basic Steps for Docker:
- First make the Dockerfile.In Docker File Setup the Working Environment e.t.c. of that app.
   For Example see the Dockerfile of this project.
- Make YML file as docker-compose.yml file. In docker-compose.yml setup about what we want store in docker container.
  For example see the docker-comopse.yml of  this project
  
  #### Starting Docker :
  - For run the project with Docker. Type 
  ``` docker-compose up ```  in the terminal.
  - For stop the project with Docker. Type 
  ``` docker-compose down ```  in the terminal.
   
  #### Making own Docker Image:
  For Example: This is a example of Sequelize/Migration project.
  - First bulid the imgae of the project locally. Type
  ```docker build . -t surajthaqurie/sequelize-mysql``` in the terminal
  - Then make conatainer locally. Type
  ```docker container run -d -p 80:3000 surajthaqurie/sequelize-mysql```.
    in the terminal. 
    ###  Here,
     - ```80``` port is used for locally and ```3000``` port is used by App.
     - ```surajthaqurie``` is your username of Docker hub.
     - And ```sequelize-mysql``` is name of container but accutally this is name of image.
    
   - Then push that image in your Docker Hub.Type
     ```  docker push surajthaqurie/sequelize-mysql```in the terminal.
    
  
  
   #### THANK YOU
