Les utilisateurs
================

.. _`utilisation_utilisateurs_niveaux`:
Les niveaux d’utilisateurs
--------------------------

Il existe 4 niveaux d’utilisateurs :

- **Niveau 3** |user_niv3|
   - C’est le plus bas niveau et le niveau par défaut d’**Info Sites**. Il ne peut qu’ajouter des sites à des projets, les modifier et voir les informations de connexion à un site s’il est lié auxdits projets. Il ne peut avoir d’action en dehors des projets auxquels il est lié.
- **Niveau 2** |user_niv2|
   - C’est le rôle qu’on donne aux utilisateurs qui doivent créer des organisations, des contacts, des projets, des sites. *Il verra les informations de connexion des projets auxquels il est rattaché.*
- **Niveau 1** |user_niv1|
   - Cet utilisateur est un administrateur. Il peut créer des utilisateurs, changer leur statut depuis l’espace d’administration. Il peut réaliser toutes les actions du niveau 2 et 3. Il a accès à toutes les informations de connexion des différents projets, même ceux auxquels il n’est pas lié.
- **Niveau 0** |user_niv0|
   - C’est le super-administrateur d’**Info Sites**. Il a tous les droits disponibles dans **Info Sites**. Il correspond au statut d’administrateur webmestre de SPIP. Il peut gérer les plugins, les organisateurs, les contacts, les projets, les sites de projets mais aussi les utilisateurs. Mais surtout, il peut faire des actions sur la base de données dans l’espace d’administration d’**Info Sites**.

.. tip::
   Il est à noter que le niveau suivant a les mêmes droits que le niveau précédent en plus des spécificités de son niveau. Par exemple, le niveau 2 peut faire les mêmes actions que le niveau 3. Ce qui n’est pas le cas inversement.
   De plus, seuls les niveaux 1 et 0 ont le droit d’accéder à l’espace d’administration.

.. _`utilisation_utilisateurs_voir`:
Voir la fiche d’un utilisateur
------------------------------
**Utilisateur(s) :** |user_niv0| |user_niv1| |user_niv2| |user_niv3|

Depuis l’espace utilisateur, chaque utilisateur peut consulter la fiche d’un autre utilisateur depuis un projet en cliquant sur le nom dudit utilisateur.

Un utilisateur de niveau 2 minimum a dans le menu *Autres* accès à l’item **Utilisateurs**. En cliquant sur cet item, l’utilisateur pourra consulter la liste de tous les utilisateurs référencés dans **Info Sites**. En cliquant sur le nom de l’utilisateur, il pourra consulter la fiche de l’utilisateur désiré et voir toutes les informations saisies pour cet utilisateur. Bien entendu, il ne pourra voir le login et le mot de passe de cet utilisateur.

.. _`utilisation_utilisateurs_page`:
Page d’un utilisateur
^^^^^^^^^^^^^^^^^^^^^
Sur la page d’un utilisateur, en dessous des éléments renseignés (voir la section *Modification d’un utilisateur*), les tableaux listent les éléments suivants :

- Les projets associés à l’utilisateur ;
- Les sites des projets auxquels l’utilisateur est associé ;
- Les commits (Git, SVN, etc.) en reprenant l’email de l’utilisateur. C’est-à-dire pour l’utilisateur ayant l’email *martin.dupont@entreprise.tld*, les commits de l’utilisateur *martin.dupont* lui seront associés.
- Tout autre entité auquel l’utilisateur a été associé.


.. _`utilisation_utilisateurs_attribuer`:
Attribuer des projets à un utilisateur
--------------------------------------
**Utilisateur(s) :** |user_niv0| |user_niv1| |user_niv2|

Sur la page d’un utilisateur, cliquer sur le bouton **Attribuer des projets à cet utilisateur** dans la colonne de droite. Sur cette nouvelle page, il est possible d'associer rapidement des projets à l’utilisateur sans passer par la page du projet. Il faut cliquer sur le rôle de l’utilisateur pour lesquels puis cliquer sur le bouton **Enregistrer**. En début de formulaire, cliquer sur **Filtres** pour voir les éléments suivants :

- **Technologie** : filtrer les projets par logiciels renseignés sur les sites des projets ;
- **Organisations** : filtrer les projets selon leur organisation ;
- **Autres**, les filtres possibles sont :
   - **Mes projets** : n’afficher que les projets auxquels l’utilisateur connecté est associé ;
   - **Projets de l’utilisateur** : n’afficher que les projets auxquels l’utilisateur est déjà associé. Cela permettra de les éditer rapidement.


.. _`utilisation_utilisateurs_modification`:
Modification d’un utilisateur
-----------------------------
**Utilisateur(s) :** |user_niv0| |user_niv1|

Depuis la page d’un utilisateur, cliquer sur le bouton **Modifier cet utilisateur**. On pourra éditer les champs suivants :

- **Signature** (obligatoire) : le nom ou le pseudo de l’utilisateur ;
- **L’adresse email** (recommandée) ;
- **Qui est cet utilisateur :** Un courte biographie sur l’utilisateur, ou tout simplement ses fonctions ;
- **Statut :** Le niveau de l’utilisateur dans **Info Sites** ;
- **Nom du site de l’utilisateur** ;
- **Adresse (URL) du site** ;
- **Login :** Le login doit contenir au moins 4 caractères ;
- **Nouveau mot de passe :** il doit contenir au moins 6 caractères et doit être renseigné 2 fois. Ces champs sont à laisser vides si on ne désire pas changer le mot de passe de l’utilisateur.

Cliquer sur le bouton **Enregistrer** pour que les modifications soient prises en compte. Une redirection vers la fiche de l’utilisateur se fera si aucune erreur de saisie est rencontrée.

.. note::
   Lorsqu’un serveur LDAP a été configuré, dans ce cas précis, le login de l’utilisateur ne peut pas être modifié. Il correspond à l'identifiant LDAP de l’utilisateur. De plus, il est déconseillé de modifier le mot de passe de l’utilisateur pour ne pas porter à confusion l’utilisateur.

.. _`utilisation_utilisateurs_role`:
Rôle d’un utilisateur sur un projet
-----------------------------------
Un utilisateur peut être associé à un projet sur lequel il travaille. Ceci est très important notamment pour les utilisateurs de niveau 3. En effet, après avoir été associé à un projet, il pourra agir sur les sites des projets, en les créant, modifiant ou si besoin les supprimant.

Les rôles possibles sont les suivants :

- Directeur de projets
- Chef de projets
- Commercial
- Référent technique
- Architecte
- Lead Développeur
- Développeur
- Intégrateur

Il est possible d’attribuer plusieurs à un utilisateur sur un même projet.


.. _`utilisation_utilisateurs_suppression`:
Suppression d’un utilisateur
----------------------------
**Utilisateur(s) :** |user_niv0| |user_niv1|

Depuis l’espace d’administration, survoler l’icone **Édition** puis cliquer sur **Utilisateurs**. Dans le tableau de listing des utilisateurs enregistrés, choisir l’utilisateur désiré en cliquant sur son nom. Puis cliquer sur **Modifier cet utilisateur**. Modifier le champ **Statut** pour la valeur *> à la poubelle*.

Cliquer sur le bouton **Enregistrer** pour que ce nouveau statut soit pris en compte. Une redirection vers la fiche de l’utilisateur se fera si aucune erreur de saisie est rencontrée.

Dans la colonne de gauche, en dessous du numéro de l’utilisateur, le statut affichera *à la poubelle*.


.. |user_niv3| image:: ../_static/user_niv3-16.png
   :alt: Niveau 3
.. |user_niv2| image:: ../_static/user_niv2-16.png
   :alt: Niveau 2
.. |user_niv1| image:: ../_static/user_niv1-16.png
   :alt: Niveau 1
.. |user_niv0| image:: ../_static/user_niv0-16.png
   :alt: Niveau 0
.. |user_supprime| image:: ../_static/user_supprime-16.png
   :alt: Supprimé
