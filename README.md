# hi
##https://stackoverflow.com/questions/3216360/merge-update-and-pull-git-branches-without-using-checkouts/17722977#17722977 
##comment faire des merges sans passer par checkout
Ca dépend un peu des cas en fait, prenons l'exemple d'un site web:
J'ai une branche production/master qui est celle hébergée sur le serveur. Celle-ci n'a même pas besoin d'être en local car le seul à l'utiliser c'est le serveur.
J'ai une branche développement qui est le miroir de celle-ci mais avec les infos de config pour pouvoir héberger et tester le site en local sur mon ordi
Enfin j'ai des sous branches "feature" pour par exemple, l'ajout d'un moyen de payement sur le site.
Lorsque je vais valider une feature, je vais la merger dans development qui sera pushé sur le repo distant. Puis je peux simplement merger development dans master sur le repo distant sans jamais y toucher sur mon ordi puisque cette branche "ne m'intéresse pas" (en local tout du moins) (edited) 
