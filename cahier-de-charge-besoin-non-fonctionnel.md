CAHIER DES CHARGES – BESOINS NON FONCTIONNELS

Projet : Application de Gestion des Notes Scolaires


1. Contexte du Projet

L’objectif du projet est de concevoir et déployer une application permettant la gestion numérique des notes des élèves.
L’application doit offrir une plateforme sécurisée, fiable et conviviale pour les enseignants, les élèves, les parents et l’administration scolaire.

Ceci  présente exclusivement les Besoins Non Fonctionnels (BNF) nécessaires au bon fonctionnement, à la performance et à la qualité globale du système.

Definition : un besoin non fonctionnel est une exigence qui décrit les caractéristiques et les contraintes d’un systeme , d’un produit ou d’un service , sans d’écrire ses fonctionnalités spécifiques.

2. Exigences Non Fonctionnelles

2.1. Performance

2.1.1. Temps de réponse

Le chargement des pages ne doit pas excéder 3 secondes.

L’affichage des bulletins ou moyennes doit se faire en moins de 2 secondes.

Les opérations de saisie ou modification d’une note doivent être instantanées (≤ 1 seconde).

2.1.2. Capacité & Charge

Le système doit supporter au moins 500 utilisateurs simultanés.

La base de données doit pouvoir gérer jusqu’à 100 000 élèves, leurs notes et historiques sur plusieurs années.

2.1.3. Disponibilité de service

L’application doit être opérationnelle 24h/24 – 7j/7, avec une disponibilité minimale de 99 %.


2.2. Sécurité

2.2.1. Authentification & Gestion des rôles

Identification par nom d’utilisateur + mot de passe sécurisé.

Gestion stricte des rôles :

Administrateur

Enseignant

Élève

Parent

Superviseur académique (option)

2.2.2. Confidentialité des données

Utilisation obligatoire du protocole HTTPS(hypertext Transfer Protocol Secure)est un protocol de communication sécurisé utilisé pour transmettre des données sur internet .

Les mots de passe doivent être stockés sous forme hachée et salée (c’est a dire les mots de passes ne doivent pas etre stockés en claire mais plutot sous une forme transformée qui les rend inutilisables pour les pirates informatiques via le hachage qui va permettre de transformer le mot de passe en une chaine de caracteres de longueur fixe).

Les données sensibles doivent être chiffrées.


2.2.3. Journalisation

Le système doit enregistrer automatiquement :

Modifications de notes

Connexions

Ajout/Suppression d’élèves ou classes

Les logs(journal de bord /enregistrement chronologique d’évenement,d’action ou de transactions qui se produisent dans un systeme ) doivent être conservés au minimum 12 mois.

2.2.4. Sauvegarde & Restauration

Sauvegarde automatique de la base chaque 24 heures.

Possibilité de restauration complète en cas d’incident.

2.3. Fiabilité

2.3.1. Tolérance aux pannes

En cas d’interruption, le système doit reprendre sans perte de données.

Mise en place d’un mécanisme de sauvegarde automatique en cours de saisie.

2.3.2. Qualité des services

Taux d’erreur acceptable < 0,5 %.

Aucun risque de duplication ou perte de notes lors des opérations critiques.


2.4. Compatibilité

2.4.1. Compatibilité Navigateurs

L’application doit fonctionner avec :

Google Chrome

Mozilla Firefox

Microsoft Edge

Safari

2.4.2. Compatibilité Mobile

Version mobile responsive disponible sur Android et iOS.

2.4.3. Intégration

Compatible avec d’autres systèmes scolaires (ex : gestion des absences, paiements).

2.5. Ergonomie et Expérience Utilisateur (UX):qui visent a créer des produits ,des systemes et des environnements qui soient faciles a utiliser, efficaces et agréables pour les utilisateurs.)

2.5.1. Interface simple & intuitive

L’utilisateur doit pouvoir effectuer ses tâches en ≤ 3 clics.

Interface adaptée pour les utilisateurs non techniciens.

2.5.2. Accessibilité

Textes lisibles, contrastés et adaptés aux déficiences visuelles.

Responsive design pour tablettes et smartphones.

2.5.3. Multilingue

Support du Français, de l’Anglais, et possibilité d’ajouter d’autres langues.

2.6. Maintenabilité

2.6.1. Standards de développement

Code propre, modulaire et respectant les bonnes pratiques du framework(cadre de travail) utilisé.

2.6.2. Documentation

Documentation technique complète :

API(interface de programmation d’application) qui va permettre de demander des services ou des données a un autre systeme, et de recevoir des réponses.

Architecture(est la conseption et la structure du systeme informatique)

Base de données

Manuel d’utilisation

2.6.3. Tests

Tests unitaires ≥ 80 % de couverture du code.

Tests de charge sur opérations critiques (importation massive de notes…).
2.7. Portabilité

Déploiement possible sur :

Serveur local (intranet)

Serveur distant

Infrastructure cloud (AWS, Azure…)

L’application doit pouvoir être migrée sans modification majeure.

2.8. Scalabilité( adaptation a des changements de charge de travail de trafic ou de données sans compromettre sa performance sa disponibilité et sa fiabilité.

Le système doit pouvoir s’étendre pour :

Plusieurs établissements scolaires

Plus d’élèves sans perte de performance

Ajout de nouvelles fonctionnalités (ex : gestion des absences, emploi du temps)

2.9. Confidentialité

Un enseignant ne voit que les notes de ses classes.

Un élève ne voit que ses propres résultats.

Un parent ne voit que les informations de son enfant.

L'administration a accès général selon son niveau d’autorisation.

2.10. Auditabilité

Toutes les modifications doivent être traçables :

Auteur de la modification

Date et heure
Ancienne valeur

Nouvelle valeur

2.11. Conformité Légale

Respect des normes de protection des données (inspiré RGPD / normes locales).

Conservation des données scolaires selon les règles pédagogiques en vigueur.

.Évolutivité: la capacité à gérer de nouvelles fonctionnalités Sans affecter la stabilité de l'application, Gérer une augmentation du nombre d'utilisateurs.

 3. Conclusion

Ce cahier des charges définit les exigences Non Fonctionnelles essentielles pour assurer :

la qualité,

la sécurité,

la performance,

la fiabilité,

et la bonne maintenance
du système de gestion de notes.

Il constitue une base solide pour encadrer le travail de l’équipe technique et garantir un produit final professionnel.

