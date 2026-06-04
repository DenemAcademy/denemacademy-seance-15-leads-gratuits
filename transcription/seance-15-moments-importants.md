# Séance 15 - Moments importants

Transcription découpée par blocs de 5 minutes. Les clés API ont été masquées.

## Repères pédagogiques

- Je pars du dossier `mon-business` et j'isole le travail dans `06-prospects`.
- Je présente Serper comme un moyen de récupérer des résultats Google Search, Google Places et Reviews via API.
- Je colle la clé dans le prompt seulement pour le run, puis elle doit être révoquée.
- Je demande à Claude Code de créer une base de leads massive, dédupliquée, scorée et exportée.
- Je vérifie les crédits, les logs, les fichiers générés, les scores et le fichier Excel final.

## Blocs de transcription

### Bloc 01 - 00:00:00 à 00:05:06

Ok, c'est parti. On commence du coup la séance numéro 15 et on va s'attaquer à la génération de l'Ids. Donc, on va utiliser l'outil Serper et ça va être totalement gratuit parce qu'ils vont nous offrir 2500 crédits. Donc, nous, ce qu'on va faire, c'est qu'on va utiliser Claude Code. Cette fois-ci, ça ne sera pas Codex. Donc, on va récupérer la commande encore une fois, YOLO Mode. Et on va aller dans Mon Business. Et cette Une fois ci, on va dans Prospect et numéro 6. Maintenant, dans le dossier, on lance la commande et c'est parti. Donc là, notre devoir faire avant de donner à code, de donner SEO, GEO, comprennent encore plus le contexte et après, on va utiliser du coup server toutes les informations que Cloudcode récupérer, on passera du coup et après, on a un fichier xlsx. Donc on va essayer d'avoir un maximum de volumes, de récupérer des glides. Encore une fois, là, vu qu'on est sur une version gratuite avec 2500 crédits, on va être limité, mais on aura quand même une belle base de données. Une fois qu'on aura, du coup, à chercher à les enrichir lors de prochaines séances. On va avoir une base très bien structurée et exploitable pour de la peau enrichir parce que là on récupère à peu près un message qu'on va faire. Du coup, ça va être une architecture qui va se dérouler comme ça. En plusieurs couches, la partie de marché, la partie ICP plus sèquement, on va faire une matrice avec les roquettes, on va chercher la partie place, donc place avec Google Maps, on va faire une partie search, des adresses, web, notre Google, nombre d'avis, catégorie, slash search, contact et la source, donc page contact, on va sur les gals annuaire, papers, calling company, snippet avec email, après on va utiliser slash reviews, pour détecter appel, réservation, attente, Slash tout complète avec un gros, ça va être tous les aides pointes qu'on utilisait en un appel. Un système de matrice, ce qu'on va faire, c'est qu'on va faire un axe segment, un axe zone, un axe intention, un axe, le segment restaurateur, le mig, gastronomie, traiteur, pizzeria, hôtel, restaurant, on va faire aussi le même segment, constamment et de pas avoir des leads, qu'on ne compte pas à Maniche, on va les faire aussi sur la zone, ville, département, région, quartier, zone touristique, ça va nous permettre de passer de 1 000 à 40 000 fiches brutes on va aller chercher aussi de l'intention, donc l'intention c'est contact, mention légal, privatif, réservation, recrutement

### Bloc 02 - 00:05:00 à 00:10:00

donc ça va nous permettre d'augmenter la chance de trouver un contact ou un signal d'achat on va faire aussi une source avec Google Business, site, annuaire, papers, n'est-ce que bien il faut pas simplement faire une seule boucle, un seul parcours, un, deux, trois, quatre et après Merci d'un autre GXLSX avec toute la mesurie, ensuite il va répéter, il va faire ça jusqu'à temps qu'on n'ait plus, et après on va faire de la déduplication, comme tout à l'heure, pour le scrapping similaire et du mode basse, donc painscore, téléphone, site, formulaire, que d'une compagnie, discord, accoutis de réservation, site, chiffres au volume d'un painscore, avec le routement et à la fin on aura du coup un GXLSX avec 12 onglets, donc dashboard, all leads avec e-mail, on aura peut-être des partis sans e-mail, une part à plus, priorité commerciale, geo, grid map, ville, département, densité, segment, tégorie, revue au signal, les douleurs détectées, les carries ledger, les requêtes et coups, les dupes maps, fusion et source, le scoring screws, même message, tature. Là, l'objectif c'est d'avoir un promis du coup xls6 avec plusieurs onglets, bien structuré, on verra en détail une fois par livrer mais l'information en rapport à cette stratégie là, en fait tout ce qu'on va voir c'est en C15, du coup celle ci c'est en C16, c'est en C17, c'est en C19, ça va être à créer là avec c'est enrichir au fur et à la stratégie que je vous montre, je mets en place pour m'éclater un maximum et ensuite avoir un lit qualifié pour ça c'est une automatisation complète plusieurs étapes que vous pouvez revendre facilement. C'est comme ça que ça se vend le plus souvent. Avec une boîte, la parmi l'EADS, si vous les enrichissez, une ligne égale, une team 901. Ça peut être une solution, proposer un service d'automatisation, une régie par exemple de panneau solaire qui est du l'EADS. Ça est un tour de business et en plus de le voir ensemble. Encore une fois, ça part d'un prompt. Il fait un maximum le travail. Je demande bien tout comprendre. Justement un prompt à copier le prompt.

### Bloc 03 - 00:10:00 à 00:18:39

Vous allez tout simplement coller juste ici et après on va le Serpereur pour aller donner une autre clé API. Donc moi j'ai un compte Serpereur, donc là je l'ai créé tout à l'heure, pas de compte Serpereur, vous allez sur le Père API, sign up et vous renseignez les informations tout simplement, vous prenez nom, adresse email et passeword, après ils vont demander une confirmation par mail, vous cliquez dessus et vous allez arriver du coup sur le dashboard. Donc moi je suis sur le dashboard, j'ai les 2500 crédits offerts, si je clique ici, on peut voir que j'ai ma clé API, donc c'est ce qu'il nous faut, donc je vais donner directement. Ensuite, on a besoin de quoi ? On a besoin de mon business, tu de marché et j'ai besoin aussi de la partie auditation. Donc là, j'ai toutes les informations. Je vais donner mon prompt, je vais donner ma clé API, je vais donner mon écune de marché et mon auditation. Là, comme vous pouvez voir, on a pu sur paramètres. On peut aller sur search, sur image, sur vidéo, sur place, Sur place, par exemple, je mets bistro, cul, c'est le mot-clé, donc la carries, moi je cherchais en France, localisation, Paris, langage, French. On ne commande pas, je souhaite voir une. Donc là, comme on peut voir, j'ai un jason avec des informations, des adresses, etc. Nous, c'est ce qu'on va faire, tourner sur 1 000, 20 000 pages en même temps. Le résultat, utiliser place, on va utiliser aussi maps. Une fois qu'on a récupéré les informations, avec l'attitude, la longitude, on va tout simplement croiser les données, comme je vous l'ai dit, pour récupérer encore plus d'informations. On va aller chercher aussi la partie reviews, donc reviews c'est quoi, c'est les avis Google, etc. Donc ça peut être intéressant justement si on voit qu'il y a des avis négatifs, on ne met jamais la clé dans les fichiers logs et que ça

### Bloc 04 - 00:15:00 à 00:19:41

est markdown, on ne la fiche jamais. Une fois, elle est consommée, la clé sera revocée. Donc Il faut bien lui dire parce que parfois il prend la tête, il va te dire que je ne veux pas me le dans le fichier VLV. Donc là c'est du one shot, prendre la tête, du volume, tu ne dois pas faire un échantillon, tu dois pousser la collecte au maximum. Viser 40 000 lits pour une, il le permette. Donc viser le maximum de lits dédupliqués, viser le maximum de lits avec email public, viser le maximum de lits à plus à exploitable commercialement. Continuez à appeler le serpeur correctement, il reste des zones, des segments, des synonymes ou sourds. seulement si le serpeur indique les quotas atteints, paiement requit ou erreur écrite.

### Bloc 05 - 00:20:00 à 00:25:12

Ok, là ils sont en train de continuer, là il fait vraiment brasserie, il fait restaurant sur toutes les villes, après il va faire tous les mots-clés donc c'est top, laisse travailler. Ne demande pas de validation entre les tours, tu avances en autonomie, crée, brife, c'est le MD, là c'est tout ce qu'il va nous faire. Donc ça, quand vous allez donner vos fichiers, va adapter. Si ton marché n'est pas la restauration, adapte totalement, c'est pour ça qu'il y a une formation là. zone construite, couverture France, top 100 des villes, Française, départements, régions, zone touristique, secondaire à Fort Siupro, variable, roquette place, segment ville, segment, c'est ce qu'on a vu là, restauration vers le segment roquette, on va voir pk, play dead point, enrichir grâce à serveur.

### Bloc 06 - 00:25:00 à 00:29:03

Là vous faudra juste payer un petit peu pour enrichir, c'est au niveau happy-fi, vous avez même une version gratuite à 5$ qui va faire l'affaire, Je suis peut-être un peu moins quand même, mais avec des outils gratuit, une bonne stratégie et avec code-code de connecté, on va avoir une bonne base et qu'il faut le faire vraiment.

### Bloc 07 - 00:30:00 à 00:30:59

Poser une question, travailler.

### Bloc 08 - 00:40:00 à 00:44:21

Et si on n'a pas toutes les informations, on utilise HappyFile du coup. Cooper aussi les lignes que j'ai, et si on a...

### Bloc 09 - 01:30:00 à 01:35:20

Donc là on va arriver à la fin du coup, comme vous pouvez voir on n'aura plus de crédit, du coup ce qu'on va faire c'est recréer un nouveau compte Serper. Déméler les phases, mentionner, faire un message, des indications supplémentaires. Je vais lui donner une nouvelle clé API Serper, donc pour ça ça va pas être compliqué. Logout, Serper, anti-mail, récupérer encore une fois la clé API. Là normalement on a 2500 crédits, dashboard, 1500, il y a la bonne clé. On demande tout simplement de refaire l'étape en question, notre plan, encore une fois, Search, Contact, Hero View Suite Arrangement, merci de là, pour réfléchir et corriger justement le système. Par rapport à ma demande, je vais leur donner une clé à pays normalement. On va repartir du coup sur cette nouvelle clé, on va voir sa réflexion, faire la phase 4, phase 5, top. On se met bien plus rapidement, cette fois-ci, la recherche, l'end point il va être différent.

### Bloc 10 - 01:35:00 à 01:36:14

Voilà ce qu'on fait, c'est ça. Rélègue l'adresse e-mail. Ce qui se passe...

### Bloc 11 - 01:45:00 à 01:47:45

Ascat du coup

### Bloc 12 - 01:50:00 à 01:54:44

Ok, donc top, on a bien en détail, mais on a 377 lits bruts, on a énormément de lits sans e-mail donc ça c'est problématique, mais cher par la suite, justement, on a parti website, Capify, c'est plutôt pas mal on a quand même les adresses e-mail, on a la fourchée prie
