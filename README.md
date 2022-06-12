# sonarqube

Levantar el servidor de sonarqube
```
docker-compose up -d
```

Para ejecutar sonar scanner debe ejecutar el siguiente comando desde la raíz del proyecto que se desea analizar

```
docker run --rm -e SONAR_HOST_URL="http://ip_local:9000" -v "$(pwd):/usr/src" sonarsource/sonar-scanner-cli
```

Nota: no de debe usar localhost como ```SONAR_HOST_URL```
