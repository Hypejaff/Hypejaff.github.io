---
date: 2017-11-29T23:00:00.000Z
layout: post
show_post: true
title: STUDYFLOW
subtitle: StudyFlow est une application mobile et web qui permet à des parents de suivre les cours particuliers de leur(s) enfant(s).
description: 
image: /assets/img/picture/studyflow-icon.png
optimized_image: /assets/img/picture/studyflow-icon.png
show_image: true
category: projet
tags:
  - JAVA
  - AndroidStudio
author: arnaudjaffrennou
paginate: true
---
[Dépôt GIT ici](https://github.com/Hypejaff/STUDYFLOW)
## Présentation de StudyFlow 
Au contact de plusieurs personnes qui donnent des cours à des élèves que le suivi des cours et que la communication entre l'élève et le professeur est parfois difficile. Ainsi par exemple provoquant du retard dans le travail que doit effectuer l’élève pour le prochain cours.
Afin de répondre à ce besoin en forte croissance, nous avons pris l’initiative de réaliser une application mobile et web multiplateforme (Smartphones, tablettes & PC)  accessible en ligne. 

> Concrètement, STUDYFLOW est une application mobile et web qui permet à des parents de suivre les cours particuliers de leur(s) enfant(s). Mais permet aussi à des professeurs de communiquer et d’avoir accès à des fonctionnalités de suivi (calendrier, échanges, envoi de devoirs, etc…). 

Le principe de l’application repose sur l'interaction entre ces deux parties afin de minimiser les pertes de temps et combler le manque de communication.

## Besoins
Dans un premier temps, notre projet vise à convaincre les professeurs particuliers et les parents pour un suivi des cours. Selon le déploiement de l’application, il n’est pas exclu de prévoir des évolutions afin de cibler un périmètre plus large.
L’application a pour objectif de faciliter le suivi des cours donnés par un professeur particulier. Il peut communiquer plus facilement avec son élève par un système de tchat. Mais également planifier ses cours par le biais d’un calendrier.

--page-break--
## L'application
Nous avons pensé de simplifier au maximum l’utilisation de l’application en séparant en partie les grandes fonctionnalités de l’application : La messagerie, le calendrier, le stockage puis profile. 
Nous avons aussi adapté notre application en fonction du marché, cette à dire l’ergonomie et le design des applications qui nous entourent.
L‘application a été développer à partir de la vue d’authentification de l’utilisateur puis la première vue au lancement de l’application et ensuite la vue principale. Le nombre d’emplacement dans la « Dashboard » de la vue principale c’est fait en fonction du nombre de fonctionnalité que l’on pouvait regrouper en partie. Nous avons commencé par la partie profile « You » de l’utilisateur pour se familiariser avec ce langage de programmation. 
Ensuite le partie messagerie « Community » qui a duré une longue période du à des problèmes rencontrés. Et enfin en parallèle, la partie stockage « Storage » et la partie calendrier « Schedule » ne sont pas finaliser car il reste quelques fonctionnalités a programmé.

### IHM du lancement de l’application
<img src="/assets/img/picture/studyflow/app1.png">

1. Au lancement de l’application, l’utilisateur peut visualiser une vue durant quelque seconde affichant le logo de l’application sans interaction sur la vue.
2. Sur cette vue qui est la page de connexion, l’utilisateur s’authentifie via son adresse électronique et son mot de passe pour se connecter à son compte en cliquant sur le bouton « Login » et continuer.
3. Sur cette vue qui est la page principale affichant les différentes parties de l’application. Nous pouvons visualiser que l’utilisateur a accès aux parties suivantes : profile, calendrier, stockage, communauté et paramètre. Ces différentes parties seront présentées ci-dessous.

### IHM de la partie messagerie
<img src="/assets/img/picture/studyflow/app2.png">

1. Dans cette vue principale, Prenons le cas où vous cliquez dans le cadre bleu-clair « Community ».
2. Sur cette vue de messagerie, l’utilisateur à l’occasion de discuter avec différentes personnes présentes dans ces contacts.
3. En cliquant sur le menu déroulant de la vue numéro deux en haut à gauche. Nous pouvons visualiser deux onglets permettant d’afficher les différentes discussions et les demandes d’ajouts. Puis en bas de ce menu un bouton permettant d’ajouter des contacts.
4. Sur cette vue qui affiche une fenêtre au centre. L’utilisateur peut ajouter des contacts par leur adresse électronique.

### IHM de la partie stockage
<img src="/assets/img/picture/studyflow/app3.png">

1. Dans cette vue principale, Prenons le cas où vous cliquez dans le cadre bleu-clair « Storage ».
2. Cette vue est démarrée automatiquement à l’appuie sur « Calendar » dans la vue principale. Sur cette vue, il est affiché les différents dossiers que l’utilisateur a de base pour classer ses différents documents.
3. Sur cette vue, il est affiché les différents documents pour chaque dossier.

### IHM de la partie profile
<img src="/assets/img/picture/studyflow/app4.png">

1. Dans cette vue principale, Prenons le cas où vous cliquez dans le cadre bleu-clair « You ».
2. Sur cette vue de profil, l’utilisateur visualise ses informations personnelles. Il peut modifier son mot de passe en cliquant sur le bouton en bas de vue « Change password ».
3. Sur cette vue qui affiche une fenêtre au centre, l’utilisateur peut modifier son mot de passe en réécrivant l’ancien mot de passe puis en écrivant deux fois le nouveau mot de passe.

### IHM de la partie calendrier
<img src="/assets/img/picture/studyflow/app5.png">

1. Dans cette vue principale, Prenons le cas où vous cliquez dans le cadre bleu-clair « Schedule ».
2. Sur cette vue de calendrier, l’utilisateur navigue dans le calendrier et peut cliquer sur différentes dates pour afficher la liste des évènements ou tâches du jour.
3. Lorsque l’utilisateur clique sur le rond bleu avec une croix blanche, une fenêtre s’ouvre au centre de la vue pour ajouter une nouvelle tâche.
4. Sur cette vue de note à faire, l’utilisateur pourra créer des notes pour lui rappeler des choses.

--page-break--
## Architecture
L’application est passée par différentes étapes avant d’en arriver au produit finis.
Pour commencer la première étape était simple : pouvoir connecter l’individu à la base de données du projet. Pour cela rien de plus simple, on peut se dire, il suffit juste de renseigner un login et un mot de passe de l’envoyer puis de recevoir une réponse permettant ou non d'accéder à la base de données. Et bien non, ce n’est pas si simple que ça, j’ai donc dû rechercher une solution pour pouvoir communiquer avec la base de données via l’application.
Après de nombreuses recherches (principalement sur internet), j’ai enfin trouvé une solution. J’ai donc utilisé ce qu’on appelle le type JSON (JavaScript Object notation), un format de texte indépendant de tout langage ainsi donc un langage d’échange de données idéal.
Cependant, il me fallait une plateforme pour que ces échanges entre l'application et la base de données soit possible, c’est ainsi que nous avons utilisé le site internet pour que ces échanges puissent avoir lieu.
Ainsi l’application allait pouvoir envoyer du JSON sous forme de requêtes POST sur une page du site auxquelles cette dernière renverra un type JSON renvoyé à son tour à l’application et enfin passer par une fonction de l’application pour en extraire tous les éléments.
Malheureusement, même si la logique de fonctionnement fut très vite appréhendée la mise en place du code mettant en action ces principes furent un peu plus complexe mais néanmoins réalisable. Une fonction permettant l’envoie de requête mais aussi une mise en forme de simples chaines de caractères en type JSON mais aussi un traitement des données JSON en retour m’ont permis de répondre à cette problématique majeure de notre projet

### Le stockage des données
#### Base de données SQL
Une fois le transfert de données établie, il faut bien stocker les valeurs renvoyées sur l’application, plus précisément sur le téléphone.
Ici aussi, du fait que je connaissais très peu la technologie sur laquelle j'évoluais j’ai donc cherché sur internet des solutions dans le but de stocker ces informations.
Dans un premier, j’ai utilisé une base de données SQL directement stockées sur le téléphone. Cette solution présente certains avantages : tout d’abord les données sont persistantes c’est à dire que même si l’application est fermée, les données créent dans la base donnée reste et sont de nouveau accessible une fois l’application relancé. 
De plus la mise en place d’une base de données SQL sur application est plutôt simple et les requêtes fonctionnent de la même manière que dans les autres outils de développement ou l’on fait des requêtes SQL.
De ce fait, la prise fut assez rapide du fait que l’on a déjà vu cette technologie au cours de notre formation.
Cependant, cette méthode présente aussi des inconvénients, dans un premier temps, le stockage. En effet, comme dit auparavant les données sont stocké directement sur l’appareil et persiste une fois l’application fermé, cela peut poser un problème car si au fur et à mesure de son développement les données prennent de plus en plus de place cela peut empêcher certain utilisateur d’utiliser l’application si ces derniers ont très d’espace de stockage. 
Alors certes, cette méthode, marche, est fonctionnelle mais elle n’est pas pratique d’utilisation. Comme je l’ai dit pour pouvoir accéder aux données stockées sur la base de données de l'application il faut faire des requêtes et ensuite savoir exactement où se trouve les informations nécessaires pour pouvoir en disposer. 
Enfin de compte ça rend le développement de l’application fastidieux car a chaque que l’on besoin d’une information il faut faire une requête et savoir ou pointer dans le résultat l’information.
C’est pour cela qu’en cour de développement, l'équipe et moi-même ont décidés de changer de méthode pour stocker les données.

#### Notion D’objet
Voulant simplifier l’utilisation des données utilisé par l’application, il fallut donc trouver une solution alternative. La problématique fut simple il fallait que les données soit créé pendant l’utilisation de l’application mais que ces derniers soient supprimés une fois l’application fermé afin de ne pas prendre de place sur l’appareil mais aussi que l’utilisation soit facile.
C’est ainsi que j’ai décidé de mettre en place la notion d’objet. Chaque objet est créé sous forme de classe java dans l’application, on renseigne ces attributs et on initialise un constructeur par défaut qui reprend les attributs renseignés.
Cette solution permet donc de créer des objets, dans le projet différents objets seront créés au cours de l’utilisation. De ce fait il a fallu créer un classe utilisateur message, conversation…
Utiliser la notion de classe et donc d’objet implique donc la notion de constructeur lorsque l’on veut ajouter un élément et pouvoir s’en servir après de ces données qui le compose.
De plus, les classes se référents aux différents objets sont facile d’utilisation, dans ce cas pas besoin de requête comme en SQL à rallonge ou il faut savoir où se trouve exactement l’information. Dans ce cas, on peut créer des fonctions get() qui vont directement nous retourner la valeur désiré.

### Fonctions principales de l'application
Une fois les données stockées et mise à la disposition, il faut bien maintenant pouvoir utiliser ces données dans l'utilisation de l’application.
Je vous invite donc à consulter l’annexe le code complet pour une plus grande compréhension globale du projet. 
Cependant voici les fonctions principales ainsi que leur explication : 

* `void onCreate(Bundle savedInstanceState);` cette fonction est appelé à chaque fois qu’une activity (fenêtre interface) est crée
*	`new RequestInternet().execute();` cette fonction est la clef de voûte de cette application. Elle est utilisée à chaque fois d’une requête POST est nécessaire par l’application 
*	`x.setOnClickListener();` est une fonction selon un élément de l’interface, par exemple un bouton xxx, et si on “clique” dans le cas présent ça sera un contact tactile on active alors le code contenu dans cette fonction. Cette fonction est très importante dans le projet car de nombreuses actions sont conditionnées selon les actions de l’utilisateur.
*	`void loadIntoBDD(String json);` cette fonction permet de créer les différents objets qui sont ensuite utilisé dans l’application.
*	`Intent intent = new Intent(Login.this, MainActivity.class);` l’objet intent de type Intent est permet de passer de l’activité Login à celle appelé MainActivity.
*	`intent.putExtra("ProfilData",Perso);` la fonction putExtra permet d’ajouter l’objet Perso sous le nom “ProfilData” dans l’objet intent précédemment créer, c’est celle qui permet la persistance des données entre les activité du fait qu’on les ajoute dans la nouvelle activité créer.
*	`startActivity(intent);` active le changement d’activité à l’autre selon l’objet Intent indiqué
*	`Intent i = getIntent();` permet de récupérer les données de via l’intent de l’activité précèdent
*	`MonProfil = (DonneeUser) i.getSerializableExtra("ProfilData");` permet de récupérer l’objet dénommé “ProfilData” c’est à dire l’objet Perso.
