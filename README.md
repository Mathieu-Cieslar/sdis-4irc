# sdis-4irc


1 Récupérer les différent composant du projet


```bash
git clone https://github.com/Mathieu-Cieslar/sdis-emergency.git
```
```bash
git clone https://github.com/Mathieu-Cieslar/sdis-simulation.git
```
```bash
git clone https://github.com/EtienneCHZ/IOT.git
```
```bash
git clone https://github.com/Mathieu-Cieslar/simulateur-microService.git
```
```bash
git clone https://github.com/Mathieu-Cieslar/emergency-microService.git
```

Créer le network docker avant de build et up le projet 

```bash
docker network create sdis-emergency
```

Lancement des containers

```bash
docker-compose up -d --build
```

Installation des dépendances sur les back web Symfony

```bash
composer install 
```
Lancement des migrations
```bash
php bin/console doctrine:migrations:migrate
```
- Le front simu est accessible sur le port 8082
- Le front emergency est accessible sur le port 8080
- Le back simu est accessible sur le port 8083
- Le back emergency est accessible sur le port 8081

- la bdd simu est sur le port 5433
- la bdd emergency est sur le port 5432



