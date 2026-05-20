# CI/CD workshop Code Foundry

## Build Your Own Pipeline (Mario & Luigi Style)
In deze kennissessie ga je zelfstandig (of samen, you can self bepil) een pipeline opzetten voor een bestaande applicatie.
Het doel is niet alleen om "iets werkend te krijgen", maar om inzicht te krijgen in:
- hoe een CI/CD pipeline is opgebouwd
- welke stappen essentieel zijn
- hoe feedbackloops het beste vormgegeven kunnen worden
- hoe je pipelines onderhoudbaar en betrouwbaar houdt.

De workshop is opgebouwd uit meerdere fases. Elke fase bouwt verder op de vorige, maar voel je te alle tijden vrij om zelf los te gaan.

### Het doel
Aan het einde van de workshop hopen wij dat jullie een pipeline hebben opgezet die:
- automatisch draait bij een push
- de applicatie build
- tests uitvoert
- een Docker image bouwt
- alleen deployed wanneer alle controles slagen
- conditioneel enkel deployed vanaf `main`

### Technische Context
#### Applicatie
Dit project bevat een eenvoudige backend applicatie gebouwd met:
- Java 21
- Spring Boot
- Gradle
- Docker

De applicatie bevat:
- REST endpoints
- Unit Tests
- Integration Tests
- Docker ondersteuning

#### Applicatie lokaal draaien
```shell
./gradlew bootRun
```

#### Tests uitvoeren
```shell
./gradlew test
```

#### Docker image builden
```shell
docker build -t cicd-workshop
```



