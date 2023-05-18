---
date: 2022-08-02T23:00:00.000Z
layout: post
show_post: true
title: Les certificats SSL
subtitle: 
description: Présentation des certificats SSL
image: /assets/img/picture/certificats/certificat.jpg
optimized_image: /assets/img/picture/certificats/certificat.jpg
show_image: false
category: article
tags:
  - Certificat
  - SSL
  - Blog
author: arnaudjaffrennou
paginate: false
---

## C’est quoi un certificat SSL?
Il est utilisé principalement pour identifier et authentifier une personne physique ou morale, mais aussi pour chiffrer des échanges de données.
Pour un site web il s'agit d'un certificat SSL. On parle de SSL pour « Secure Sockets Layer », c'est un protocole de sécurité qui crée un lien chiffré entre un serveur Web et un navigateur Web.

Pour simplifier, le protocole HTTPS est une extension de HTTP. Le « S » à la fin est l’initiale signifiant « Secure ». 
La plupart des navigateurs signalent les sites HTTP (ceux qui n'ont pas de certificat SSL) comme étant « non sécurisés ». C'est une façon claire de signaler aux utilisateurs que le site peut être dangereux, et cela pousse les entreprises à migrer vers une adresse HTTPS. Nous pouvons également constater la présence d’un petit cadenas à côté de l'URL dans la barre d'adresse, cela veut dire que le SSL protège le site Web que vous visitez.
<img src="/assets/img/picture/certificats/certificat-presentation.png">

## Pourquoi les avoir ?
Les sites Web ont besoin de certificats SSL pour sécuriser les données des utilisateurs, vérifier qui est le propriétaire du site Web, empêcher les criminels de créer une version frauduleuse du site et obtenir la confiance des utilisateurs.
Les certificats SSL assurent la confidentialité des interactions en ligne et l'authenticité du site Web pour que les utilisateurs puissent partager leurs informations privées en toute confiance.
Pour les entreprises, il faut savoir qu'un certificat SSL est requis pour obtenir une adresse Web HTTPS. HTTPS est la forme sécurisée d'une adresse HTTP, cela signifie que les sites Web en HTTPS ont un trafic protégé par le protocole SSL. 


## Les caractéristiques des certificats SSL
* L’url du site à certifier 
* Les coordonnées de votre entreprise
* Votre clé publique 
Une clé cryptographique est alors mis en place sur les deux communicants pour pouvoir s’identifier et échanger.
* Le nom de l’Autorité de Certification, qui émet ce passeport électronique
Une autorité de certification (CA) est une organisation qui vend des certificats SSL/TLS à des propriétaires web, à des sociétés d'hébergement web ou à des entreprises. 
L'autorité de certification valide le domaine et les détails du propriétaire avant d'émettre le certificat SSL/TLS. 
Pour être une autorité de certification, une organisation doit répondre à des exigences spécifiques définies par la société du système d'exploitation, des navigateurs ou des appareils mobiles et demander à être répertoriée en tant qu'autorité de certification racine. 
Ce point est important pour établir la confiance entre les utilisateurs.
* La signature de l’Autorité de Certification
* La date d’expiration de ce certificat SSL
pour ajouter une sécurité supplémentaire au protocole en renouvelant les clés cryptographique au bout d’une certaine date.

## Les types de certificats SSL
Il existe trois types de certificats SSL. Les niveaux de chiffrement sont les mêmes pour chaque type de certificat. Ce qui diffère, ce sont les processus d'audit et de vérification nécessaires pour obtenir le certificat.

L'Autorité de Certification (AC) vérifie que l'organisation en question possède le droit exclusif d'utilisation du nom de domaine et soumet celle-ci à un audit.

* Certificats à validation étendue (EV)
Les certificats EV SSL sont disponibles pour tous types d'entreprises, que ce soit des agences gouvernementales et des entreprises enregistrées ou non constituées en société. Des critères obligatoires que l'AC doivent remplir afin de pouvoir émettre des certificats SSL à validation étendue. Un audit vérifiant que ces critères sont bien remplis est conduit chaque année.
* Certificats à validation de l'organisation (OV)
L'AC vérifie que l'organisation en question possède le droit exclusif d'utilisation du nom de domaine pour lequel elle souhaite recevoir le certificat et soumet celle-ci à certaines vérifications. Les informations vérifiées apparaissent également dans le sceau de site sécurisé, pour une confiance accrue de la part des visiteurs. Le nom de l’organisation apparait également dans le certificat sous le champ ON.
* Certificats à validation de domaine (DV)
L'AC vérifie que l'organisation en question possède le droit exclusif d'utilisation du nom de domaine pour lequel elle souhaite recevoir le certificat. L'identité de l’entreprise ne fait l’objet d’aucune vérification particulière. Aucune information n’apparait donc dans le sceau de site sécurisé, mis à part les informations relatives au chiffrement. Vous avez la garantie que vos informations sont chiffrées, mais vous ne pouvez pas être sûr de savoir qui est réellement le destinataire de ces informations.

## Fonctionnement d'un certificat SSL
<img src="/assets/img/picture/certificats/certificat-fonctionnement.png">
