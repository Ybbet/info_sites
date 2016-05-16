---------------
Configurer SPIP
---------------
Après avoir récupérer les fichiers sources de SPIP, dans votre navigateur, aller à l'adresse suivante : `http://example.tld/ecrire/`. Et suivre les différentes étapes à l'écran.

Cela fait, aller sur la page de gestion des plugins : ``Configuration > Gestion des plugins``. Puis cliquer sur ``Verrouilés``. Rechercher le plugin ``SVP``. Cliquer sur l'icône de configuration à droite de la ligne. Cela vous amènera sur la page ``http://example.tkd/ecrire/?exec=configurer_svp``. Sélectionner les éléments suivants dans le formulaire :

.. code-block:: html

   Activer le mode runtime ? 'Non'
   Activer le mode pas-à-pas ? 'Non'
   Activer les logs verbeux ? 'Non'
   Autoriser l'activation des paquets obsolètes ? 'Non'
   Permettre l'édition des dépôts ? 'Non'

Cliquer sur ``Enregistrer`` après avoir sélectionné 'Non' à chaque élément.

~~~~~~~~~~~~~~~~
Ajouter un dépôt
~~~~~~~~~~~~~~~~
* Revenir sur la page de gestion des plugins : ``Configuration > Gestion des plugins`` ;
* Cliquer sur l'onglet ``Ajouter des plugins > Dépôts`` ;
* Dans le formulaire ``Ajouter un dépôt``, saisir le lien ``http://plugins.spip.net/depots/principal.xml`` dans le champ ``Fichier XML du dépôt`` ;
* Cliquer sur le bouton ``Ajouter``.

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Installer le plugin Info Sites
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
* Aller sur la page de gestion des plugins : ``Configuration > Gestion des plugins`` ;
* Cliquer sur l'onglet ``Ajouter des plugins > Plugins`` ;
* Dans le champ ``Rechercher dans les plugins``, taper *info sites* ;
* Sélectionner ``Tous les états`` dans le champ ``États`` ;
* Cliquer sur le bouton ``Rechercher`` ;
* Cocher la case correspondant à la ligne ``Info Sites`` ;
* Puis cliquer sur le bouton ``Télécharger et activer`` ;
* Enfin, valider la fenêtre de dialogue pour lancer l'installation du plugin et de ses dépendances ;
* Recharger la page si nécessaire.

