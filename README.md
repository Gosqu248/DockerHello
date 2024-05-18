Example project in Maven to learn Docker 

Command that I used in this

docker build .         
building image / budowanie obrazu 

docker build -t urban/docker-hello:v2 .       
building image with name REPOSITORY: urban/docker-hello  and TAG: v2 / budowanie obrazu z nazwą Repozytorium: urban/docker-hello oraz Tag: v2

docker images  
check available images / sprawdzenie dostępnych obrazów

docker ps  
check all the docker containers / sprawdzenie wszystkich dockerowych kontenerów

docker run -p 8080:8080 32c  
-p 8080:8080  <-- set port as 8080
run docker container with name starting with name 32c on port 8080 / uruchomienie dockerowego kontenera z nazwą zaczynającą się od 32c na porcie 8080 

docker run -p 7777:8080 -e user=tester 32c 
run docker container with environment variables "user" sets as "tester" on port 7777 / uruchomienie contenera ze zmienną środowiskową "user" jako "tester" na porcie 7777

docker run -d -p 9999:8080 -e user=developer 32c 
-d <-- detached mode 
run docker container with environment variables "user" sets as "developer" on port 9999 / uruchomienie contenera ze zmienną środowiskową "user" jako "developer" na porcie 9999
