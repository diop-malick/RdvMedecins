# Learning project
# Electoral systems Application for Proportional representation

Application client / serveur de prise de rendez-vous pour un cabinet medical avec plusieurs medecins. 



# Architecture

Client / serveur -> 4 Modules  :

	* rdvmedecins-api-core				(DAO, métier / Spring Data JPA Hibernate , Spring Securité)
	* rdvmedecins-api-ws					(REST web service / Spring MVC)
	* rdvmedecins-api-web-springmvc		(ui web / Spring MVC & thymeleaf)
	* rdvmedecins-api-web-jsf			(ui web / JSF 2 et primeface)
	
	* rdvmedecins-api-web-angularjs		(ui web / AngularJS 1)
		(projet angular à part , généré avec yeoman, importer dans un projet maven web)
	
# Stack Technique

* Plateform : JDK 1.8
* Object Lifecycle & IOC : Sprig boot / Spring 4
* Test : JUnit 4
* DAO : Spring Data JPA / Hibernate
* Web Service : Spring MVC
* Security	: Spring Security
* UI : Spring MVC (web) / Angular JS / JSF 2

Côté serveur, on utilise les technologies
[Spring Data] pour l'accès à la base de données*;
[Spring MVC] pour le service web*;
[Spring Security] pour la sécurisation de celui-ci*;
[Mysql] - Pour le SGBD

# Outils utilisés

* IDE : Eclipse Mars (+ Spring Tools Suite)
* Application Server : Tomcat 7
* SCM : Git
* Build : Maven 3
* SGBD : WampServer (MySQL 5) - Workbench

# Features

l'utilisateur se connecte et 
peut ensuite choisir le médecin avec lequel on veut un rendez-vous [2] et le jour de celui-ci [3] 
voir l'agenda du médecin choisi pour le jour choisi ;
une fois obtenu l'agenda du médecin, on peut réserver un créneau
Une fois le rendez-vous validé, on est ramené automatiquement à l'agenda où le nouveau rendez-vous est désormais inscrit. Ce
rendez-vous pourra être ultérieurement supprimé

i18n  : FR & EN

# Link

Tutoriel :
	
	* http://tahe.developpez.com/java/spring/serge-tahe-spring-mvc-rest-security-cors-angularjs-tutoriel-debutant/
		

# accée :
api				:  localhost:8080
ui-client-cors	:  localhost:8081/client.html
	