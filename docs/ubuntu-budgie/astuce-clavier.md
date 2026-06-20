#### Astuce pour Ubuntu Budgie 24.04.

À l'installation d'Ubuntu Budgie 24.04, j'ai rencontré le problème suivant :
- Lors du choix du clavier (Bépo sans pavé numérique pour moi), les options pour les claviers Bépo correspondaient toutes à des claviers étendus.

**Conséquence :** lors de l'affichage de la page d'ouverture de session, le clavier numérique n'est pas activé, mais une fois la session ouverte il est automatiquement activé. Or cela ne me convient pas puisqu'alors une partie des touches ne fonctionne plus.

Pour modifier cela, j'ai dû :
- éditer en mode superutilisateur le fichier : /etc/default/numlockx
- modifier la ligne : NUMLOCK=auto en NUMLOCK=off
- enregistrer, bien sûr, la modification.

*Remarque : cette astuce peut aussi servir pour les ordinateurs portables sans pavé numérique.*
