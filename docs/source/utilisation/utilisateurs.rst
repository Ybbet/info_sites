Les utilisateurs
================

Les niveaux
-----------

Il existe 4 niveaux d’utilisateurs :

- **Niveau 3** |user_niv3|
   - C’est le plus bas niveau et le niveau par défaut d’**Info Sites**. Il ne peut qu’ajouter des sites à des projets, les modifier et voir les informations de connexion à un site s’il est lié auxdits projets. Il ne peut avoir d’action en dehors des projets auxquels il est lié.
- **Niveau 2** |user_niv2|
   - C’est le rôle qu’on donne aux utilisateurs qui doivent créer des organisations, des contacts, des projets, des sites. *Il verra les informations de connexion des projets auxquels il est rattaché.*
- **Niveau 1** |user_niv1|
   - Cet utilisateur est un administrateur. Il peut créer des utilisateurs, changer leur statut depuis le back office. Il peut réaliser toutes les actions du niveau 2 et 3. Il a accès à toutes les informations de connexion des différents projets, même ceux auxquels il n’est pas lié.
- **Niveau 0** |user_niv0|
   - C’est le super-administrateur d’**Info Sites**. Il a tous les droits disponibles dans **Info Sites**. Il correspond au statut d’administrateur webmestre de SPIP. Il peut gérer les plugins, les organisateurs, les contacts, les projets, les sites de projets mais aussi les utilisateurs. Mais surtout, il peut faire des actions sur la base de données dans le back office.

.. tip::
   Il est à noter que le niveau suivant a les mêmes droits que le niveau précédent en plus des spécificités de son niveau. Par exemple, le niveau 2 peut faire les mêmes actions que le niveau 3. Ce qui n’est pas le cas inversement.
   De plus, seuls les niveaux 1 et 0 ont le droit d’accéder au back office.

Création d’un utilisateur
-------------------------
**Utilisateur(s) :** |user_niv0| |user_niv1|

Depuis l’espace d’administration, survoler l’icone **Éditions** puis cliquer sur **Utilisateurs**. Dans la colonne de gauche ainsi qu’en bas de la page, cliquer sur le bouton **Créer un nouvel utilisateur**. On pourra y saisir les informations suivantes :

- **Signature** (obligatoire) : le nom ou le pseudo de l’utilisateur ;
- **L’adresse email** (recommandée) ;
- **Qui cet utilisateur :** Un courte biographie sur l’utilisateur, ou tout simplement ses fonctions ;
- **Statut :** Le niveau de l’utilisateur dans **Info Sites** ;
- **Nom du site de l’utilisateur** ;
- **Adresse (URL) du site** ;
- **Login :** Le login doit contenir au moins 4 caractères ;
- **Nouveau mot de passe :** il doit contenir au moins 6 caractères et doit être renseigné 2 fois.

.. note::
   Lorsqu’un serveur LDAP a été configuré, la création d’un compte utilisateur se fait automatiquement lorsque cet utilisateur s’identifie pour la première fois à **Info Sites**. Dans ce cas précis, les utilisateurs de niveau 0 et 1 ne doivent pas créer de compte pour ledit utilisateur depuis l’espace d’administration pour ne pas se déroger à LDAP.


Modification d’un utilisateur
-----------------------------

Suppression d’un utilisateur
----------------------------


.. |user_niv3| image:: ../_static/user_niv3-16.png
.. |user_niv2| image:: ../_static/user_niv2-16.png
.. |user_niv1| image:: ../_static/user_niv1-16.png
.. |user_niv0| image:: ../_static/user_niv0-16.png
.. |user_supprime| image:: ../_static/user_supprime-16.png
