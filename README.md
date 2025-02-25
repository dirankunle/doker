My microservices Project

(ability to run multiple container -run frontend backend together)

The 3 microservices
  - database
  -  wordpress image
  -  phpadmin

Docker compose Tool : is the file used to run multiple container

1. create a directory for docker compose
2. create network
 - the docker compose file is sectionized: version, container service, Volume for persistence and network

Step1: Pull and run images from central docker repo 
      eg. -docker run -itd -p 3000:3000 Grafana/grafana
step2: create volume for persistence
       create path for the volume
step3: create restart policy
step4: create environment variable - for authorization
step5: create loop 
   - depends-on for retainability 
step 6: create ports for each services to listen on 

Note: the naming must follow this nomenclature: docker-compose.yml 

and run docker compose up -d
    to power up all your services at once
  -d will make your project run in daemon mode
