## Consignes

Source : [lien vers l’énoncé du challenge](https://ctf.challenge-osint.fr/user/missions/boxes?uuid=f1483c91-03ba-445a-9bb4-22a015690815)

<img width="1389" height="771" alt="Capture-consignes" src="https://github.com/user-attachments/assets/2f148ce9-485e-41dc-a4f1-9cb4e7576c5c" />

---

## Étape par étape la résolution

### Étape 1 – Identifier le contexte via une recherche d’image inversée

- J’utilise la recherche par image de [Google Images](https://www.google.com/imghp?hl=FR) avec la photo de street art fournie.
- Parmi les résultats, je clique sur un article du site [linfo.re](https://www.linfo.re/la-reunion/societe/rendez-vous-avec-jace).
- L’article indique que l’artiste de ce street art est **Jace**, un artiste français, et qu’il a réalisé une série de graffitis à **Tchernobyl**.

---

### Étape 2 – Confirmer la localisation et obtenir un indice supplémentaire (« Jupiter »)

- Je poursuis avec Google Images en combinant la recherche par image et le mot-clé **« Tchernobyl »**.
- Je trouve une page sur [ArtMajeur.fr](https://www.artmajeur.com/katalina-tattoo/fr/oeuvres-d-art/15567751/chernobyl-ukraine-zone) où la même œuvre est photographiée par **Catalina Tatou**.
- Dans la description, elle précise qu’il s’agit d’un graffiti situé sur **l’un des murs du “coucher de soleil de Jupiter”** à Tchernobyl.

---

### Étape 3 – Identifier « Jupiter » comme une usine à Pripyat

- À partir des mots-clés **« Jupiter »** et **« Tchernobyl »**, j’effectue une recherche Google classique.
- Dans les résultats (notamment sur des banques d’images comme [Dreamstime](https://fr.dreamstime.com/usine-jupiter-%C3%A0-pripyat-tchernobyl-zone-ukraine-atelier-l-ancienne-ville-abandonn%C3%A9e-d-exclusion-image215919452)), je trouve des légendes du type « usine de Jupiter à Pripyat, Tchernobyl, zone Ukraine ». 
- « Jupiter » correspond donc à une **usine** située à **Pripyat**, dans la zone de Tchernobyl.

---

### Étape 4 – Récupérer les coordonnées de l’usine Jupiter 

- Je recherche **« usine Jupiter Pripyat »** sur Google.
- Je clique sur la page [Wikipédia](https://fr.wikipedia.org/wiki/Jupiter_(usine)) dédiée à l’usine Jupiter.
- Je récupère les **coordonnées géographiques** indiquées pour ce site : 51° 24′ 09″ N, 30° 02′ 32″ E

---

### Étape 5 – Repérer le mur dans Street View (première date)

- J’ouvre ces coordonnées dans **Google Maps**.
- Je passe en mode **Street View** autour de l’usine Jupiter.
- Je place le bonhomme sur les points accessibles et j’explore les alentours du bâtiment abandonné.
- En comparant l’architecture (forme du mur, ouvertures, environnement) avec la photo du challenge, j’identifie un mur correspondant, mais **sans le graffiti**.
- La vue Street View affichée est datée de **2015**.

<img width="1598" height="1257" alt="Capture-1" src="https://github.com/user-attachments/assets/9c648c7a-3803-413b-a0ab-c369c29542f5" />

---

### Étape 6 – Utiliser l’historique Street View pour trouver une vue avec le graffiti

- Depuis le point Street View identifié j’ouvre d’abord l’historique.
- Je constate que la vue Street View la plus récente disponible est datée de 2020. Cette vue contient le graffiti, mais elle ne correspond pas à la date attendue par le challenge (septembre 2021).

Pour obtenir une date plus récente, j'essaye de modifier le positionnement de mon avatr dans Street View :
- soit en suivant les lignes bleues (Street View classique),
- soit en ciblant les points ronds bleus (photosphères).

À proximité du bâtiment de l’usine Jupiter, je repère un point photosphère, indépendant de la ligne Street View.
En entrant dans cette photosphère, j’accède à une vue datée de septembre 2021, où le graffiti est visible.

Les informations associées à la photosphère indiquent le nom et le prénom de l’auteur de la prise de vue : c’est la réponse attendue par le challenge.
  
<img width="2241" height="1266" alt="Capture-resultat" src="https://github.com/user-attachments/assets/eab6ef1b-db6a-4ea2-8d28-f6168abb6cd2" />



