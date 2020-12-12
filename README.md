# Exo 2 du jour3 de la semaine 5

# a) Niveau facile
Quel est le nombre total d'objets Album contenus dans la base (sans regarder les id bien sûr) ?
- 347
- Album.count

Qui est l'auteur de la chanson "White Room" ?
- Eric Clapton
- Track.find_by(title: 'White Room')

Quelle chanson dure exactement 188133 milliseconds ?
- Prefect
- Track.find_by(duration: 188133)

Quel groupe a sorti l'album "Use Your Illusion II" ?
- nil
- Track.find_by(album: "Use Your Illusion II")

# b) Niveau Moyen
Combien y a t'il d'albums dont le titre contient "Great" ? (indice)
- 13
- Album.where("title like '%Great%'").count

Supprime tous les albums dont le nom contient "music".
- Album.destroy_by("title like '%music%'")

Combien y a t'il d'albums écrits par AC/DC ?
- 2
- Album.where("artist like '%AC/DC%'").count

Combien de chanson durent exactement 158589 millisecondes ?
- 0
- Track.where("duration like '%158589'").count

# c) Niveau Difficile
==Pour ces questions, tu vas devoir effectuer des boucles dans la console Rails. C'est peu commun mais c'est faisable, tout comme dans IRB.==

puts en console tous les titres de AC/DC.



