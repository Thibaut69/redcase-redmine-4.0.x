
Redcase
=======

Test case management plug-in for Redmine
----------------------------------------

Redcase allows you to create, manage, and execute test cases, group them into
test suites, link them with the native Redmine issues, work with multiple test
environments, create reports, and more.

Please see the project's [Wiki](https://bitbucket.org/bugzinga/redcase/wiki) for
more information.

[FR]

A installer comme un plugin classique, décompresser l'archive dans le répertoire plugin et renommer le dossier simplement "redcase".
Ensuite lancer la mise à jour de la base de données (faire un backup auparavant !) pour ajouter les tables nécessaires au plugin avec cette commande :

*bundle exec rake redmine:plugins:migrate RAILS_ENV=production*

Redémarrer le serveur applicatif (Puma ou autre)

Ensuite, ajouter les trackers "Test Case" à vos projets et aussi le tracker "Bug" si vous ne l'avez pas (utile pour rapporter un bug sur un test non concluant).

Bon à savoir : Pour déplacer les cas de tests dans l'onglet "Test Case", il est nécessaire que ces derniers soient au statut "In Progress".

[EN]

Install like any other plugin, unzip or untar the file in the plugin directory and rename the folder simply "redcase".
Then launch the update of your database (do a backup before !) to add the news tables used by the plugin with this command :

*bundle exec rake redmine:plugins:migrate RAILS_ENV=production*

Restart your application server (Puma or other)

Then, add the trackers "Test Case" to your projects and also the tracker "Bug" if you don't have it yet (useful to report a bug when a test is not OK).

Nice to know : To drag and drop the tests case in the "Test Case" tab, they need to be at status "In Progress".
