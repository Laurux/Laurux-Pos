 Installation. 
        Laurux3 et Laurux3.Pos sont disponibles sous forme de deux fichiers exécutables séparés.
        Laurux3.Pos est dépendant de Laurux3, c'est en quelque sorte un module extérieur. Il faut donc impérativement que l'installation de Laurux3 soit faite et que le logiciel soit opérationnel, sinon la caisse ne fonctionnera pas.
        La base est commune pour les deux logiciels. Donc, une sauvegarde copiera l'ensemble des données du système de gestion et des caisses.
        Dans le répertoire Laurux3.pos il existe un dossier Doc_Caisse qu'il faut copier sous le répertoire Laurux3 car Laurux3 utilise aussi une partie de cette documentation.
        Il faudra créer un lanceur sur le bureau qui chainera sur le programme Laurux3.pos.gambas situé sous le répertoire Laurux3.pos. A ce lanceur vous pouvez associer l'icône "caisse.png" situé sous ce même dossier.

        Le module point de vente de Laurux3 est activé par l'option   "Gestion des caisses"  dans l'onglet  "Gestion (2)"  dans les préférences. Lorsque cette option est activée alors on aura une entrée supplémentaire ("Caisse") dans le menu de Laurux3.

        Deux types de configurations sont possibles.

        1- Monoposte.  

        Après extraction de l'archive Laurux3 on aura un repertoire nommé "Laurux3" qui contiendra l'ensemble des programmes et des documentations Laurux3. Ce repertoire est créé automatiquement à l'installation de Laurux3. 
        Après extraction de l'archive Laurux3.Pos on aura un autre repertoire nommé "Laurux3.Pos" qui contiendra l'exécutable (Laurux3.Pos) et un sous repertoire ("Doc_Caisse") qui contiendra la documentation de la caisse. Il faudra dupliquer ce dossier sous le répertoire Laurux3 car Laurux3 utilise aussi cette documentation.

        2- Réseau.  

        Par commodité, je nomme serveur le poste sur lequel se trouve la base MySQL et Laurux3. Le poste client (ou la caisse) étant celui ou sera copié Laurux3.Pos.

        Sur le serveur on aura l'installation classique de Laurux3, c'est à dire qu'on aura un repertoire nommé "Laurux3" qui contiendra l'ensemble des fichiers nécessaire à son fonctionnement (Voir la doc d'installation de Laurux3). Sous ce repertoire, on copiera aussi la documentation de Laurux3.Pos, donc on aura un nouveau chemin nommé "Doc_Caisse" contenant tous les fichiers Html et Png de la documentation.
        NB: On copie la documentation de Laurux3.Pos car Laurux3 utilise aussi cette documentation.

        Sur la caisse, après extraction de l'archive "Laurux3.Pos" on aura un repertoire nommé "Laurux3.Pos" qui contiendra l'exécutable (Laurux3.Pos) et un sous repertoire ("Doc_Caisse") qui contiendra la documentation.

        Concernant MySQL, il faut installer les paquets server et client sur la caisse car dans un proche avenir Laurux3.Pos pourra fonctionner en mode autonome.

    Utilisation.  

       En premier, il faut aller sous Laurux3 puis dans les préférences afin d'activer l'option caisse. Ceci fait, il faut ensuite aller dans le menu "Caisse" afin de créer toutes les constantes, c'est à dire les caisses puis les caissières et le client caisse et enfin le libellé bas de ticket ainsi que le libellé des avoirs.
         La première utilisation de la caisse ouvrira une fenêtre de configuration.  Il faudra bien saisir l'adresse du serveur MySQL c'est à dire l'adresse du poste sur lequel fonctionne Laurux3. Donc localhost en configuration monoposte et autre chose en configuration réseau.
