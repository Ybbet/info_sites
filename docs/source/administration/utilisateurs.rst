
Les utilisateurs
================

Les niveaux
-----------

Voir le paragraphe :ref:`utilisation_utilisateurs_niveaux`


Voir la fiche d’un utilisateur
------------------------------
**Utilisateur(s) :** |user_niv0| |user_niv1| |user_niv2| |user_niv3|

**Espace utilisateur**

Depuis l’espace utilisateur, chaque utilisateur peut consulter la fiche d’un autre utilisateur depuis un projet en cliquant sur le nom dudit utilisateur.

Un utilisateur de niveau 2 minimum a dans le menu *Autres* accès à l’item **Utilisateurs**. En cliquant sur cet item, l’utilisateur pourra consulter la liste de tous les utilisateurs référencés dans **Info Sites**. En cliquant sur le nom de l’utilisateur, il pourra consulter la fiche de l’utilisateur désiré et voir toutes les informations saisies pour cet utilisateur. Bien entendu, il ne pourra voir le login et le mot de passe de cet utilisateur.


Création d’un utilisateur
-------------------------
**Utilisateur(s) :** |user_niv0| |user_niv1|

Depuis l’espace d’administration, survoler l’icone **Édition** puis cliquer sur **Utilisateurs**. Dans la colonne de gauche ainsi qu’en bas de la page, cliquer sur le bouton **Créer un nouvel utilisateur**. On pourra y saisir les informations suivantes :

- **Signature** (obligatoire) : le nom ou le pseudo de l’utilisateur ;
- **L’adresse email** (recommandée) ;
- **Qui cet utilisateur :** Un courte biographie sur l’utilisateur, ou tout simplement ses fonctions ;
- **Statut :** Le niveau de l’utilisateur dans **Info Sites** ;
- **Nom du site de l’utilisateur** ;
- **Adresse (URL) du site** ;
- **Login :** Le login doit contenir au moins 4 caractères ;
- **Nouveau mot de passe :** il doit contenir au moins 6 caractères et doit être renseigné 2 fois.

Cliquer sur le bouton **Enregistrer** pour compléter la création de l’utilisateur.

.. note::
   Lorsqu’un serveur LDAP a été configuré, la création d’un compte utilisateur se fait automatiquement lorsque cet utilisateur s’identifie pour la première fois à **Info Sites**. Dans ce cas précis, les utilisateurs de niveau 0 et 1 ne doivent pas créer de compte pour ledit utilisateur depuis l’espace d’administration pour ne pas se déroger à LDAP.


Modification d’un utilisateur
-----------------------------
**Utilisateur(s) :** |user_niv0| |user_niv1|

Depuis l’espace d’administration, survoler l’icone **Édition** puis cliquer sur **Utilisateurs**. Dans le tableau de listing des utilisateurs enregistrés, choisir l’utilisateur désiré en cliquant sur son nom. Puis cliquer sur **Modifier cet utilisateur**. On pourra éditer les champs suivants :

- **Signature** (obligatoire) : le nom ou le pseudo de l’utilisateur ;
- **L’adresse email** (recommandée) ;
- **Qui cet utilisateur :** Un courte biographie sur l’utilisateur, ou tout simplement ses fonctions ;
- **Statut :** Le niveau de l’utilisateur dans **Info Sites** ;
- **Nom du site de l’utilisateur** ;
- **Adresse (URL) du site** ;
- **Login :** Le login doit contenir au moins 4 caractères ;
- **Nouveau mot de passe :** il doit contenir au moins 6 caractères et doit être renseigné 2 fois.

Cliquer sur le bouton **Enregistrer** pour que les modifications soient prises en compte. Une redirection vers la fiche de l’utilisateur se fera si aucune erreur de saisie est rencontrée.

.. note::
   Lorsqu’un serveur LDAP a été configuré, dans ce cas précis, le login de l’utilisateur ne peut pas être modifié. Il correspond à l'identifiant LDAP de l’utilisateur. De plus, il est déconseillé de modifier le mot de passe de l’utilisateur pour ne pas porter à confusion l’utilisateur.



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
