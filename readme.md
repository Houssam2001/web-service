# Guide pour Créer un Service Web SOAP et le Tester

Ce guide vous explique les étapes nécessaires pour créer un service Web SOAP et le tester de deux manières différentes : à l'aide de SOAP UI et d'une application côté client.

## Étapes de Création du Service Web SOAP


### 1. Création des Classes Java

- Créez les classes Java nécessaires pour implémenter vos opérations SOAP.
- Utilisez des annotations comme `@WebService` pour indiquer que les classes sont des services web.

### 2. Génération des Descripteurs WSDL

- Générez un descripteur WSDL à l'aide d'outils tels que JAX-WS ou Apache CXF.
- Le descripteur WSDL décrit la structure et les opérations du service.

### 3. Implémentation de la Logique Métier

Implémentez la logique métier à l'intérieur des méthodes de vos classes de service web.

### 4. Déploiement du Service Web

- Déployez votre service web sur un serveur d'application Java tel que Apache Tomcat ou Glassfish.
- Assurez-vous que le service est accessible via une URL.
![Screenshot 2024-02-10 at 16.59.32.png](ws%2FScreenshot%202024-02-10%20at%2016.59.32.png)
## Test du Service Web SOAP

### Méthode 1 : Utilisation de SOAP UI

1. Lancez SOAP UI et créez un nouveau projet.
![Screenshot 2024-02-10 at 17.00.35.png](ws%2FScreenshot%202024-02-10%20at%2017.00.35.png)
2. Importez le fichier WSDL de votre service web dans SOAP UI.
![Screenshot 2024-02-10 at 17.01.10.png](ws%2FScreenshot%202024-02-10%20at%2017.01.10.png)
3. Utilisez SOAP UI pour appeler les opérations du service avec différentes entrées et examinez les réponses pour vérifier le bon fonctionnement.
![Screenshot 2024-02-10 at 17.01.23.png](ws%2FScreenshot%202024-02-10%20at%2017.01.23.png)
### Méthode 2 : Application Côté Client

1. Créez une application Java côté client.
2. Utilisez les outils fournis par Java, comme JAX-WS, pour générer des classes clientes à partir du fichier WSDL de votre service web.
3. Utilisez ces classes générées pour appeler les opérations du service web à partir de votre application.
4. Vérifiez les résultats pour vous assurer que les appels fonctionnent correctement.

