Configuration requise
=====================
Pour installer **SPIP** et **Info Sites**, vous devez avoir la configuration minimale suivante sur votre serveur :

* Serveur Apache ou compatible >= 1.2 ;
* PHP >= 5.3 ;
* MySQL >= 5.0 ;
* SQLite >= 3.0 ;

Extensions PHP
--------------
* apache2handler ;
* apc ;
* apcu ;
* bcmath ;
* bz2 ;
* calendar ;
* Core ;
* ctype ;
* curl ;
* date ;
* dba ;
* dom ;
* ereg ;
* exif ;
* fileinfo ;
* filter ;
* ftp ;
* gd ;
* gettext ;
* hash ;
* iconv ;
* json ;
* libxml ;
* mbstring ;
* mcrypt ;
* mhash ;
* mysql ;
* mysqli ;
* openssl ;
* pcre ;
* PDO ;
* pdo_mysql ;
* pdo_sqlite ;
* Phar ;
* posix ;
* readline ;
* Reflection ;
* session ;
* shmop ;
* SimpleXML ;
* soap ;
* sockets ;
* SPL ;
* sqlite3 ;
* standard ;
* sysvmsg ;
* sysvsem ;
* sysvshm ;
* tokenizer ;
* wddx ;
* xdebug ;
* xml ;
* xmlreader ;
* xmlwriter ;
* Zend OPcache ;
* zip ;
* zlib.

Les modules Apache
------------------
* core ;
* http_core ;
* mod_access_compat ;
* mod_alias ;
* mod_auth_basic ;
* mod_authn_core ;
* mod_authn_file ;
* mod_authz_core ;
* mod_authz_host ;
* mod_authz_user ;
* mod_autoindex ;
* mod_deflate ;
* mod_dir ;
* mod_env ;
* mod_filter ;
* mod_log_config ;
* mod_logio ;
* mod_mime ;
* mod_negotiation ;
* mod_php5 ;
* mod_rewrite ;
* mod_setenvif ;
* mod_so ;
* mod_socache_shmcb ;
* mod_ssl ;
* mod_status ;
* mod_unixd ;
* mod_version ;
* mod_watchdog ;
* prefork.

Le serveur
----------
En cas de besoin, vous pouvez lancer l'installation des modules suivants sur votre serveur :

* curl ;
* libapache2-mod-php5 ;
* php5-apcu ;
* php5-cli ;
* php5-common ;
* php5-curl ;
* php5-gd ;
* php5-json ;
* php5-mcrypt ;
* php5-mysql ;
* php5-sqlite ;
* php5-xdebug ;
* wget.

De même, taper ces quelques lignes sur le serveur:

.. code-block:: shell

   a2enmod rewrite
   a2enmod ssl
