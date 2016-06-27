Télécharger SPIP
================


Manuellement
------------
`SPIP`_ fournit une archive zip pour permettre son installation. Vous pouvez la télécharger à cette `adresse`_.

Une fois que vous avez récupéré l'archive, vous devez la décompresser et copier le contenu de l'archive dans le répertoire qui contiendra votre site de supervision.


Automatiquement
---------------
Il est possible d'installer `SPIP`_ par le biais d'un fichier PHP : `spip_loader.php`_. Il faudra enregistrer ce fichier à la racine de votre site de supervision puis de l'appeler dans votre navigateur : `http://example.tld/spip_loader.php`. Cela fait, veuillez suivre la procédure affichée à l'écran.

.. note::
   Par défaut, le fichier `spip_loader.php` indique la dernière version stable de SPIP. Si vous désirez utiliser une autre version, vous devez modifier ce fichier en recherchant le terme **_CHEMIN_DEFINE_ZIP**. Depuis la version **2.5.7**, vous pouvez trouver en commentaire dans ce fichier les 3 branches maintenues de SPIP. A vous de choisir la version qui vous convient.


Structure des fichiers
----------------------
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

Il faut maintenant créer quelques répertoires pour que l'installation soit simplifiée. Aller dans le répertoire où vous avez installé les sources de SPIP et créer les répertoires suivants à la racine du site :

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

.. caution::
   Si vous rencontrez des problèmes d'autorisation sur les répertoires dans les étapes suivantes, il faudra changer les droits sur des répertoires avec cette ligne de commande :
      .. code-block:: shell

         chmod -R 755 local/ tmp/ config/ IMG/ plugins/ lib/


.. On renseigne ici tous les liens de la page
.. _SPIP: http://www.spip.net/fr
.. _adresse: http://www.spip.net/fr_download
.. _spip_loader.php: http://www.spip.net/spip-dev/INSTALL/spip_loader.php
