# Archipelago Manual pour Wikimasters

## CE RANDOMIZER NE SE CONNECTE EN AUCUN CAS AU SERVEUR DU JEU

**Aucune connexion, d'aucune manière, à aucun moment.**

**La validation des thèmes est manuelle** : vous cochez vous-même vos thèmes
dans le client, exactement comme on coche une liste sur une feuille de papier
avec un crayon.

---

Randomizer Archipelago pour **Wikimasters**, un jeu de cartes en ligne gratuit
où chaque carte vient d'un article de Wikipédia.

Le principe : vous ouvrez des paquets pour obtenir des cartes, et dans ce
randomizer vous devez tirer des cartes qui correspondent aux **thèmes** de la
partie pour valider des checks.

Site officiel : **https://www.wiki-masters.com/**

---

## Aucune connexion au serveur du jeu

**Archipelago Manual pour Wikimasters ne se connecte EN AUCUN CAS et d'AUCUNE
MANIÈRE au serveur de WikiMasters.**

- Le randomizer ne contacte **que** le serveur Archipelago, celui qui héberge
  la partie multijoueur. Jamais le serveur du jeu.
- Il ne lit, ne modifie et n'interagit avec **rien** sur le site
  wiki-masters.com : ni votre compte, ni vos cartes, ni vos paquets, ni votre
  progression.
- Il n'y a **aucun script, aucune extension, aucun automatisme** : rien qui
  tourne sur le site ou à côté de lui.
- La validation des thèmes est **entièrement manuelle**. C'est vous qui cochez
  vos thèmes dans le client Archipelago, un par un, comme on coche une liste
  sur une feuille de papier avec un crayon. Rien n'est validé automatiquement
  à votre place.
- Le randomizer ne vous donne **aucune carte, aucun paquet, aucun avantage en
  jeu**. Vous jouez à WikiMasters exactement comme d'habitude.

---

## Aucune affiliation

Ce projet est un **projet de fan indépendant et personnel**.

**Je ne suis en aucun cas affilié à WikiMasters** : ni au site, ni à l'équipe
qui le fait, ni à ses modérateurs, ni à qui que ce soit d'autre lié au jeu.
Je ne les représente pas, je ne parle pas en leur nom, et ils n'ont validé ni
ce projet ni ce randomizer.

Je ne suis affilié ni à Wikipédia ni à la Wikimedia Foundation, dont le contenu
encyclopédique est simplement réutilisé sous licence libre CC BY-SA.

---

## Le jeu est gratuit, n'y dépensez pas d'argent

WikiMasters est gratuit. Vous n'avez besoin d'aucun achat pour jouer à ce
randomizer : ni paquets payants, ni monnaie premium, ni quoi que ce soit.

N'achetez rien pour ça, ce serait idiot. Un compte gratuit suffit.

---

## Installer l'apworld

1. Téléchargez le fichier `manual_wikimasters_satanos.apworld`.
2. Placez-le dans le dossier `custom_worlds/` de votre installation
   Archipelago (par exemple `Archipelago/custom_worlds/`).
3. Relancez le launcher et le client. Le jeu apparaît dans la liste des mondes
   sous le nom **Wikimasters**.

Il n'y a rien d'autre à installer : pas de ROM, pas de patch, pas de logiciel
supplémentaire.

---

## Comment jouer

Au début de la partie, vous recevez **3 thèmes tirés au hasard**. Ils sont
déjà dans votre inventaire, donc les 3 checks correspondants sont tout de
suite accessibles.

Ensuite, à vous d'ouvrir des paquets sur WikiMasters et de piocher des cartes
qui correspondent aux thèmes de la partie. Chaque carte qui correspond à un
thème vous fait gagner l'item `Thème "..."` du même nom, ce qui valide le
check associé.

Vous gagnez la partie quand vous avez réuni le nombre de thèmes demandé.

Le hasard a une grande place : les thèmes actifs sont tirés à la seed, et les
items sont éparpillés dans le multiworld. Selon la chance que vous avez, une
partie peut être plus ou moins longue à finir.

---

## Contenu

Le monde contient **50 thèmes différents**. À chaque partie, un certain nombre
d'entre eux est retenu (voir les options), les autres sont retirés avec leurs
checks.

Les 50 thèmes :

- "Genre" ou "espèce" en description
- Amphibien ou reptile
- Animal
- Année dans le titre
- Années 2000
- Années 50
- Années 60
- Années 70
- Années 80
- Années 90
- Arbre sur l'image
- Avant JC
- Bâtiment
- Carte R
- Carte SR
- Cinéma
- Club sportif
- Compétition
- D'Afrique
- D'Amérique latine
- D'Asie
- D'Italie ou d'Espagne
- De Belgique ou Hollande
- De Scandinavie
- Drapeau ou écusson en image
- Du Canada
- Du Royaume-Uni
- Espace
- Guerre
- Histoire & Art (hors mus. & litt.)
- Homonymie
- Image en N&B
- Insecte ou autre bestiole
- JV & Informatique
- Lieu des USA
- Lieu polonais ou allemand
- Littérature
- Milieu Aqueux
- Mode ou textile
- Motorisé & routes
- Musique
- Nombre dans le titre (hors année)
- Pas de description
- Politique
- Radio ou télé
- Santé
- Science hors santé
- Truc qui vole (hors espace)
- Un sportif
- Végétal

---

## Options

Les options sont en français, dans l'onglet **WikiMasters** de votre yaml.

### Nombre de thèmes

Combien de thèmes sont utilisés dans la partie, parmi les 50.

- De **4** à **50**
- Par défaut : **50** (tous les thèmes)

Les thèmes non retenus disparaissent de la partie, avec leurs checks. Le
tirage est refait à chaque seed, donc deux parties ne jouent pas les mêmes
thèmes.

Le minimum est 4 et pas 1 : vous démarrez déjà avec 3 thèmes, il en faut donc
au moins un à trouver.

### Pourcentage de thèmes pour gagner

Le pourcentage des thèmes de la partie qu'il faut obtenir pour débloquer le
check de victoire.

- De **25 %** à **100 %**
- Par défaut : **75 %**

Le résultat est arrondi au supérieur. Quelques exemples :

| Nombre de thèmes | Pourcentage | Thèmes à obtenir |
|---|---|---|
| 50 | 75 % | 38 |
| 29 | 75 % | 22 |
| 20 | 50 % | 10 |
| 4 | 25 % | 4 |

Le minimum est toujours de 4 thèmes (vos 3 de départ plus 1), pour éviter
qu'une partie soit déjà gagnée au démarrage.

---

## Testé, mais à faire en async

L'apworld a été testé et fonctionne.

Ceci dit, comme tout repose sur le tirage des thèmes et sur la chance des items
dans le multiworld, une partie peut traîner en longueur. Il est fortement
conseillé de jouer en **async** plutôt qu'en session synchronisée, pour ne pas
bloquer les autres joueurs si vous attendez un thème.

---

## Crédits

Randomizer créé par **Satanos** pour Archipelago, d'après le jeu WikiMasters
(https://www.wiki-masters.com/), dont le contenu encyclopédique est issu de
Wikipédia sous licence libre CC BY-SA.

**Projet de fan indépendant, sans aucune affiliation avec WikiMasters, son
site, son équipe ou ses modérateurs, ni avec Wikipédia ou la Wikimedia
Foundation.** Ce randomizer ne se connecte à aucun moment au serveur du jeu et
ne modifie rien sur le site.
