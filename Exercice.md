1: Créer un worflow qui lors d'un push sur main:
- Build l'image docker
- Push l'image docker sur le registry
- Ajouter un multi-platform build
- Ajouter un système de cache

2: Récuperer la branche ci de grpc-task-manager
- Créer un workflow qui se déclanchera lors d'un push sur la branche ci
- Lancer, via un service, un conteneur mongodb
- Intaller les dépendances de l'app nestjs (pnpm)
- installer golang (v 1.21) puis les dépendances de test (go mod download)
- Lancer le serveur task-api dans le background
- Lacer les test (go test)
- (bonus) via les option attendre que le mongodb soit up