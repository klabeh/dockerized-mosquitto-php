# dockerized-mosquitto-php

1. First Start
    docker-compose up -d
    
    
2. We need the Container ID from eclipse:mosquitto
    docker ps
    
3. Start Shell with Container ID from Step 2    
    docker exec -it CONTAINERID_ECLIPSE_MOSQUITTO /bin/ash
    
4. Set Username & Password for Connections to Mosquitto (Anonymous is disabled)
    mosquitto_passwd -b /mosquitto/config/passwd MYUSERNAME MYPASSWORD
    
5. Restart docker Containers
    docker-compose restart