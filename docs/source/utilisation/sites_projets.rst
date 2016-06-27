Les sites de projets
====================

Voir la fiche d’un site de projet
---------------------------------
**Utilisateur(s) :** |user_niv0| |user_niv1| |user_niv2| |user_niv3|

Depuis l’espace utilisateur, cliquer sur **Sites** dans la barre de navigation pour accéder à la page listant tous les sites de projet référencés dans **Info Sites**.  Le tableau contient les éléments suivants:

* Titre des projets ;
* Le type de site ;
* Nom du logiciel ;
* Version du logiciel ;
* L’URL du Front Office.

Type de site d’un projet
------------------------
Chaque site de projet a un type déterminant son environnement :

* Local (01local)
* Développement (02dev)
* Intégration (03inte)
* Tests (04test)
* Recettes (05rec)
* Pré-production (06prep)
* Production (07prod)

Il est important de bien noter cette information pour structurer le cycle de vie d’un site. Un projet pouvoir avoir un ou plusieurs sites de types différents. *Un site de projet ne peut toutefois avoir qu’un type d’environnement.*

Création d’un site de projet
----------------------------
**Utilisateur(s) :** |user_niv0| |user_niv1| |user_niv2| |user_niv3|

Depuis la page d’accueil d’**Info Sites**, le tableau de bord, cliquer sur le bouton **Ajouter un site**.  On pourra éditer les champs suivants :

- **Titre (obligatoire)**
- **Type de site (obligatoire)**
- **Unique ID :** Une clé d'identification permettant de récupérer la configuration du serveur du site enregistré. Cette clé est de type UUID
- **Url du Web Service :** URL pour un suivi de configuration du site.
- **Date de création :** sous la forme JJ/MM/AAAA
- **Descriptif**
- *Front office :*
   - **Url du Front Office**
   - **Identifiant du Front Office**
   - **Mot de passe du Front Office**
- *Back office :*
   - **Url du Back Office**
   - **Identifiant du Back Office**
   - **Mot de passe du Back Office**
- *Logiciel :*
   - **Nom du logiciel (obligatoire)**
   - **Version du logiciel (obligatoire)**
   - **Numéro de révision**
   - **Jeu de caractères**
   - **Plugins du logiciel**
- *Les auteurs :*
   - **Administrateurs**
   - **Webmestres**
- *Serveur du site :*
   - **Nom du serveur**
   - **Port du serveur**
   - **Chemin du site sur le serveur**
   - **Logiciel du serveur**
   - **Surveillance du serveur**
- *Apache :*
   - **Modules Apache :** cette liste contient tous les modules actifs d’Apache, séparés par une virgule.
- *PHP :*
   - **Version de PHP**
   - **Mémoire allouée à PHP**
   - **Extensions PHP :** cette liste contient toutes les extensions de PHP, séparés par une virgule.
   - **Fuseau horaire**
- *Gestionnaire de versions :*
   - **Type de versioning :** SVN, CVS, Git, etc.
   - **Chemin du dépôt**
   - **Trac du dépôt**
- *Système d'accès sécurisé (SAS) :*
   - **Protocole de connexion :** FTP, SFTP, etc.
   - **Serveur SAS**
   - **Port**
   - **Identifiant**
   - **Mot de passe**
- *Informations sur la SGBD :*
   - **Type de SGBD :** MySQL, Oracle, Microsoft SQL Server, MongoDB, etc.
   - **Version de la SGBD**
   - **Serveur SGBD**
   - **Port**
   - **URL du gestionnaire de SGBD**
   - **Nom de la SGBD**
   - **Préfixe des tables**
   - **Jeu de caractères**
   - **Collation**
   - **Identifiant**
   - **Mot de passe**
- *Autres :*
   - **SSO**
   - **Périmètre d'accès**
   - **Outils de statistiques**
   - **Moteur de recherche :** Moteur interne au logiciel, Exalead, Google, etc.
   - **Autres outils**
   - **Remarques :** Caractéristiques particulières, fonctionnalités, etc.

.. note::
   Un utilisateur de niveau 3 ne peut créer, éditer et supprimer un site de projet que sur les projets auxquels il est associé.
   De la même façon, cet utilisateur ne peut pas voir les identifiants et mots de passe des sites des projets auxquels il n'est pas associé.


Règles de saisies
-----------------
**Pour les plugins du logiciel**

Saisir la liste des plugins du site en respectant les règles suivantes :

- Un plugin par ligne ;
- Le préfixe, le numéro de version, le titre complet et le statut du plugin seront séparés par un pipe "|" ;
- Pas de raccourcis typographiques de SPIP, ni de code html.

**Pour les comptes utilisateurs**

Saisir la liste des administrateurs et super-administrateurs (webmestres) du site en respectant les règles suivantes :

- Un administrateur par ligne ;
- L’identifiant, le login, l’email et le nom seront séparés par un pipe "|" ;
- Pas de raccourcis typographiques de SPIP, ni de code html.


Modification d’un site de projet
--------------------------------
**Utilisateur(s) :** |user_niv0| |user_niv1| |user_niv2| |user_niv3|

Suppression d’un site de projet
-------------------------------
**Utilisateur(s) :** |user_niv0| |user_niv1| |user_niv2| |user_niv3|


.. |user_niv3| image:: ../_static/user_niv3-16.png
.. |user_niv2| image:: ../_static/user_niv2-16.png
.. |user_niv1| image:: ../_static/user_niv1-16.png
.. |user_niv0| image:: ../_static/user_niv0-16.png
.. |user_supprime| image:: ../_static/user_supprime-16.png
