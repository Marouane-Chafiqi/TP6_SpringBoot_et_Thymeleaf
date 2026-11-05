# TP 6 : Spring Boot et Thymeleaf

Application web de gestion d'utilisateurs réalisée avec Spring Boot, Spring Data JPA, Thymeleaf et MySQL.

## Objectif

Ce TP permet de créer une application web dynamique avec Spring Boot et Thymeleaf. L'application permet d'afficher la liste des utilisateurs et d'en ajouter de nouveaux grâce à un formulaire avec validation.

## Technologies utilisées

- Java 17
- Spring Boot 3.3.5
- Spring Web
- Spring Data JPA (Hibernate)
- Thymeleaf
- Bean Validation
- MySQL
- Lombok
- Maven

## Prérequis

- JDK 17
- Maven
- MySQL
- IntelliJ IDEA

## Structure du projet

```
src/main/java/com/example/demo
├── DemoThymeleafApplication.java
├── controller
│   └── UserController.java
├── entity
│   └── User.java
└── repository
    └── UserRepository.java

src/main/resources
├── application.properties
└── templates
    ├── user-list.html
    └── add-user.html
```

## Lancement

Démarrer MySQL, puis lancer l'application :

```
mvn spring-boot:run
```

ou exécuter la classe `DemoThymeleafApplication` depuis l'IDE.

L'application est accessible sur : http://localhost:8080

## Fonctionnalités

- Affichage de la liste des utilisateurs (`/`)
- Ajout d'un utilisateur (`/adduser`)
- Validation des champs `nom` et `email` (`@NotBlank`)
- Affichage des messages d'erreur dans le formulaire

## Captures d'écran

### Liste des utilisateurs (vide)
<img width="634" height="486" alt="Capture d&#39;écran 2026-11-05 192438" src="https://github.com/user-attachments/assets/a591ac18-f3c7-4c92-a79a-4abbead68915" />


### Formulaire d'ajout
<img width="630" height="524" alt="Capture d&#39;écran 2026-11-05 192450" src="https://github.com/user-attachments/assets/4e7cbd24-ba95-4f0c-b947-86c7050d19dc" />


### Liste après ajout
<img width="611" height="430" alt="Capture d&#39;écran 2026-11-05 192458" src="https://github.com/user-attachments/assets/9b9d4e19-4833-44d8-aeff-2760214148f9" />


### Base de données MySQL (table `users`)
<img width="644" height="355" alt="Capture d&#39;écran 2026-11-05 192629" src="https://github.com/user-attachments/assets/dfaf5581-601c-4e09-abf2-e505cfeb82b9" />


