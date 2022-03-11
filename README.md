# sonarqube
El siguiente comando debe de ejecutarse desde la raiz del proyecto que se desea analizar

```
docker run --rm -e SONAR_HOST_URL="http://ip_local:9000" -v "$(pwd):/usr/src" sonarsource/sonar-scanner-cli
```

Nota: no de debe usar localhost como ```SONAR_HOST_URL```
