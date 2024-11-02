## SonarQube with Jenkins
```sh
docker compose -f docker-compose-jenkins.yaml up --build
```
---
## Execute SonarScanner manually
```sh
docker compose -f docker-compose-sonar-scanner.yaml up -d
```
```sh
docker compose ps
```
```sh
docker compose run sonarscanner
```
## Execute SonarScanner automatically
Uncomment the docker-compose code and adjust the parameters in the conf.properties of the project root
```sh
docker compose -f docker-compose-sonar-scanner.yaml up --build
```