Installation
============

Pour installer InfoSites, il vous faut installer en tout premier lieu SPIP et faire une ou deux configurations pour qu'InfoSites puissent s'installer dans les meilleurs conditions.
InfoSites est compatible avec SPIP 3.0 à minima.

----------------
Télécharger SPIP
----------------
~~~~~~~~~~~~
Manuellement
~~~~~~~~~~~~
`SPIP`_ fournit une archive zip pour permettre son installation. Vous pouvez la télécharger à cette `adresse`_.

Une fois que vous avez récupéré l'archive, vous devez la décompresser et copier le contenu de l'archive dans le répertoire qui contiendra votre site de supervision.


~~~~~~~~~~~~~~~
Automatiquement
~~~~~~~~~~~~~~~
Il est possible d'installer `SPIP`_ par le biais d'un fichier PHP : `spip_loader.php`_. Il faudra enregister ce fichier à la racine de votre site de supervision puis de l'appeler dans votre navigateur : `http://example.tld/spip_loader.php`. Cela fait, veuillez suivre la procédure affichée à l'écran.

.. note::
   Par défaut, le fichier `spip_loader.php` indique la dernière version stable de SPIP. Si vous désirez utiliser une autre version, vous devez modifier ce fichier en recherchant le terme ``_CHEMIN_DEFINE_ZIP``. Depuis la version ``2.5.7``, vous pouvez trouver en commentaire dans ce fichier les 3 branches maintenues de SPIP. A vous de choisir la version qui vous convient.


~~~~~~~~~~~~~~~~~~~~~~
Structure des fichiers
~~~~~~~~~~~~~~~~~~~~~~
Quelque soit la méthode de récupération des sources de SPIP, vous aurez une structure de fichiers telle que ceci :

.. code-block:: shell

   CHANGELOG.txt
   config/
   COPYING.txt
   ecrire/
   htaccess.txt
   IMG/
   index.php
   INSTALL.txt
   local/
   plugins-dist/
   prive/
   rien.gif
   spip.php
   spip.png
   squelettes-dist
   svn.revision
   tmp/

Il faut maintenant créer quelques répertoires pour que l'installation soit simplifier. Aller dans le répertoire où vous avez installé les sources de SPIP et créez les répertoires suivants à la racine du site :

.. code-block:: bash

   lib/
   plugins/
   plugins/auto

La nouvelle structure de répertoire sera :

.. code-block:: shell

   CHANGELOG.txt
   config/
   COPYING.txt
   ecrire/
   htaccess.txt
   IMG/
   index.php
   INSTALL.txt
   lib/
   local/
   plugins-dist/
   plugins/
   plugins/auto
   prive/
   rien.gif
   spip.php
   spip.png
   squelettes-dist
   svn.revision
   tmp/

.. warning::
   Si vous rencontrez des problèmes d'autorisation sur les répertoires dans les étapes suivantes, il faudra changer les droits sur des répertoires avec cette ligne de commande : ``chmod -R 755 local/ tmp/ config/ IMG/ plugins/ lib/``


----------------
Configurer SPIP
----------------
Après avoir récupérer les fichiers sources de SPIP, dans votre navigateur, aller à l'adresse suivante : `http://example.tld/ecrire/`. Et suivez les différentes étapes à l'écran.

Cela fait, allez sur la page de gestion des plugins : ``Configuration > Gestion des plugins``. Puis cliquez sur ``Verrouilés``. Recherchez le plugin ``SVP``. Cliquez sur l'icône de configuration à droite de la ligne. Cela vous amènera sur la page ``http://example.tkd/ecrire/?exec=configurer_svp``. Sélectionnez les éléments suivants dans le formulaire :

.. code-block:: html

   Activer le mode runtime ? 'Non'
   Activer le mode pas-à-pas ? 'Non'
   Activer les logs verbeux ? 'Non'
   Autoriser l'activation des paquets obsolètes ? 'Non'
   Permettre l'édition des dépôts ? 'Non'

Cliquez sur ``Enregistrer`` après avoir sélectionné 'Non' à chaque élément.

~~~~~~~~~~~~~~~~
Ajouter un dépôt
~~~~~~~~~~~~~~~~
* Revenir sur la page de gestion des plugins : ``Configuration > Gestion des plugins`` ;
* Cliquez sur l'onglet ``Ajouter des plugins > Dépôts`` ;
* Dans le formulaire ``Ajouter un dépôt``, saisir le lien ``http://plugins.spip.net/depots/principal.xml`` dans le champ ``Fichier XML du dépôt`` ;
* Cliquez sur le bouton ``Ajouter``.


.. On renseigne ici tous les liens de la page
.. _SPIP: http://www.spip.net/fr
.. _adresse: http://www.spip.net/fr_download
.. _spip_loader.php: http://www.spip.net/spip-dev/INSTALL/spip_loader.php
