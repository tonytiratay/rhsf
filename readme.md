### Sur le bandeau du haut : 

> tu avais proposé d’intervenir « à la main » pour centrer les modules en hauteur et les aligner sur la droite (à l’exception du logo RHSF). Penses-tu pouvoir faire ça cette semaine ? 

Du coup je vais te laisser le faire, comme on s'est dit :)

> Je crois que tu avais aussi proposer de regarder comment faire en sorte qu’un clic sur le logo RHSF mène vers la page d’accueil déconnectée et non vers « l’ancien site » (ou alors tu me disais que c’était tout à fait impossible à cause du template ?). 

Pour faire ce que vous voulez du bandeau du hait, je ne vois qu'une solution, le faire entièrement à la mano.

À l'heure actuelle, il est composé de différentes positions qui sont créées dans l'administration du template. C'est donc lui qui gere ce qui se passe au clic sur le logo.

Pour remèdier à ça, il faudrait supprimer toutes les positions du template, pour n'en laisser qu'une dans laquelle vous mettrez un module contenu personnalisé.

### Exemple

Dans ce contenu, vous pouvez vous même mettre tous les éléments désirés:

* Une image cliquable pour le logo
* Le module de recherche
* Le module de connexion
* Le module de langue

Un module contenu personnalisé se comporte exactement comme un article. Il faudrait donc passer en mode html, et créer une structure qui ressemble à ça

```html
<div class="bandeauHaut">

  <div class="logoBandeau">
    <a href="http://www.rhsansfrontieres.org/fr/entreprises" >
      <img src="adresse/de/Limage.jpg">
    </a>
  </div>

  <div class="rechercheBandeau">
    {{ nomDumoduleDeRecherche }}
  </div>

  <div class="rechercheBandeau">
    {{ nomDumoduleDeConnexion }}
  </div>

  <div class="rechercheBandeau">
    {{ nomDumoduleDeTraduction }}
  </div>


</div>

```

Les classes ci dessus (bandeauHaut, logoBandeau etc.) n'existent pas. Il faudrait donc les créer dans l'admin du template, dans le CSS personnalisé.

Pour que tous vos éléments s'alignent bien, je ne vois que l'utilisation du système de flexbox. Je ne peux pas vous faire un cours complet sur ce que sont les flexbox, aussi voici quelques liens qui devraient pouvoir vous aider:

* https://www.youtube.com/playlist?list=PLdlcrLtifCUnQ9BaCRvkiobHuSzyVApey
* https://www.youtube.com/watch?v=LNqBKTeeiWo
* https://www.youtube.com/watch?v=Mkza0N8NiK4



### Sur le bandeau du bas : 

> sais-tu comment supprimer les modules de langue et de connexion, et la mention « Free Joomla templates by AgeThemes » ?


jkhkjh


### Pop-up connexion : 

> je n’arrive pas à appliquer le nouveau template à cette pop-up. Si je ne me trompe pas, il faudrait que l’article qui s’affiche dans la pop-up soit rattaché à un lien de menu auquel le template serait assigné. Mais lorsque je vais dans la catégorie correspondante (« Articles pop up »), les liens parents qui me sont proposés sont des liens publiés. Je pensais la rattacher au menu hide, mais ça ne semble pas possible. Peux-tu m’expliquer comment faire ?

dfdgdf

### Page d’accueil déconnecté : 

> j’aimerais réduire la hauteur de la grande photo. Le format de la photo que j’ai chargée devrait le permettre, mais je ne trouve pas les paramètres pour régler ça. Comment dois-je faire ? Et aurais-tu une idée pour rendre les textes et logos sur cette photo plus lisibles ? J’ai augmenté l’ombre des textes, assombri la photo de fond. Si jamais tu as d’autres idées/astuces, je suis intéressée !

### Page d’accueil connecté (Club des mécènes) : 

> je n’arrive pas à mettre en forme le composant LinkedIn. J’aimerais qu’il n’y ait plus les barres de défilement (hauteur comme largeur). Sais-tu comment faire ? Et si possible, j’aimerais également avoir une hauteur fixe : si le texte devait dépasser cette hauteur, il serait coupé et il y aurait 3 petits points. On pourrait aussi supprimer la possibilité de faire apparaître les photos, pour éviter que ça dépasse trop vers le bas.
En parallèle, pour l’amélioration du nouveau visuel cartes-pays : j’ai fait quelques nouvelles modifications sur l’article Discriminations et harcèlement de la catégorie Qatar.

sdfsdf

> Comment peut-on baisser les titres de catégorie qui s’affichent dans les menus à gauche des cartes pays ? « Qatar » apparaît trop haut en haut à gauche. J’aimerais également agrandir la taille de police.

zfze

- De la même manière, j’aimerais abaisser la date de dernière modification qui apparaît en haut de l’article et qui mord sur le menu. Est-il également possible d’ajouter automatiquement à cette fonction d’affichage de la date la mention « Dernière révision le » ?

zefzefz