# Démonstration basique de OpenAPI

Nous allons générer du code Node.js à partir d'un fichier OpenAPI 3.0.0.

D'abord il faut installer le package `openapi-generator-cli` :

```bash
npm install @openapitools/openapi-generator-cli -g
```

Ensuite, on peut générer le code à partir du fichier `openapi.yaml` :

```bash
openapi-generator-cli generate -i openapi.yaml -g nodejs-express-server -o ./generated-server
```

Démarrage du serveur :

```bash
cd generated-server
npm install
npm start
```