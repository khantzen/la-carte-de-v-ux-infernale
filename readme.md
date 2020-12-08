La carte de vœux infernale
==================

### Introduction

Ce kata est une adaptation du [Greeting Kata](https://github.com/testdouble/contributing-tests/wiki/Greeting-Kata) pour les fêtes de fin d'année, l'objectif est de coder un générateur de texte de carte de vœux.

### Instruction

- Les itérations doivent être implémentées les une à la suite des autres sans anticipation.
- Une itération est validée si le code répond à ce qui y est spécifié ainsi que ce qui a été spécifié dans les itérations précédentes.
- L'énoncé se veut le plus "métier" possible et n'a pas pour but de vous influencer dans vos choix techniques

#### Itération 1

- Ecrire une fonction qui lorsqu'elle reçoit un prénom en entré doit souhaiter une Bonne Année à cette personne.

```
vœux(Louise) -> Bonne année, Louise.
```

#### Itération 2

- Lorsque la fonction reçoit un paramètre null ou vide en entré alors elle doit retourner un texte par défault.

```
vœux("" || null) -> Bonne année mes amis.
```

#### Itération 3

- Nous avons souvent un ami que l'on adore tellement que nous écrivons son prénom en majuscule, dans ce cas la fonction devra hurler une bonne année à cette personne.

```
vœux(ISHAM) -> BONNE ANNÉE ISHAM!
```

#### Rétro

À ce moment il peut être bon de prendre un petit moment pour se poser les questions suivante

- Est ce que je comprends ce que fait mon code ?
- Serais-je en mesure de comprendre ce que fait mon code dans un mois ?
- Qu'est ce que je pense de mon code ?
- Qu'est ce que mon code pense de moi ?
- Est ce que je peux rajouter une nouvelle fonctionnalité sans rien casser ?

#### Itération 4

- Parfois nous désirons souhaiter une bonne année à un couple d'amis ainsi quand deux prénoms sont passés en paramètre de la fonction celle-ci doit souhaiter une bonne année à ces deux personnes.

```
vœux(Louis Mouna) -> Bonne année, Louis et Mouna.
```

#### Itération 5

- Nous voulons donner la possibilité aux utilisateurs de pouvoir également souhaiter une bonne année à plusieurs personne sur une même carte de vœux.

```
vœux(Jean Karim Nicolas) -> Bonne année, Jean, Karim et Nicolas.
vœux(Haddock Tchang Tintin Milou) -> Bonne année, Haddock, Tchang, Tintin, Nestor et Milou.
```

#### Itération 6

- Il peut également arriver que nous aimons énormément un groupe d'amis. Dans le cas où tous les prénoms sont en majuscule nous désirons alors hurler une bonne année à tous ces gens

```
vœux(MAX FATMA ZAID DIMITRI) -> BONNE ANNÉE MAX FATMA ZAID ET DIMITRI!
vœux(MOUNA LOLA) -> BONNE ANNÉE MOUNA ET LOLA!
```

#### Rétro

Tout comme précédemment

- Est ce que je comprends ce que fait mon code ?
- Serais-je en mesure de comprendre ce que fait mon code dans un mois ?
- Qu'est ce que je pense de mon code ?
- Qu'est ce que mon code pense de moi ?
- Est ce que je peux rajouter une nouvelle fonctionnalité sans rien casser ?

#### Itération 7

- Dans notre groupe d'amis, il peut arriver que l'on aime certains amis plus que d'autre nous avons donc tendance à écrire leur prénom en majuscule au détriment de ceux des autres. Dans ce cas, nous souhaitons d'abord une bonne année à nos amis puis hurlons une bonne année aux autres.

```
vœux(David LOIC Fatma Morgan) -> Bonne année, David, Fatma et Morgan. ET BONNE ANNÉE LOIC!
vœux(YOHAN Lou CHARLOTTE Henry JOHANA PHILLIPE) -> Bonne année, Lou et Henry. ET BONNE ANNÉE YOHAN CHARLOTTE JOHANA ET PHILLIPE!
```

#### Itération 8

- Afin d'améliorer la fluidité de lecture nous avons décidé que désormais les prénoms devaient apparaître par ordre alphabétique sur la carte de vœux.

```
vœux(Clément Albert) -> Bonne année, Albert et Clément.
vœux(YOHAN Lou CHARLOTTE Henry JOHANA PHILLIPE) -> Bonne année, Henry et Lou. ET BONNE ANNÉE JOHANA PHILLIPE ET YOHAN! 
```

#### Itération 9

- L'utilisateur a désormais possibilité de renseigner le genre des personnes à qui il souhaite une bonne année, nous avons donc décider de faire apparaitre les femmes en premieres sur la carte de vœux.

```
vœux(Louis♂ Johana♀) -> Bonne année, Johana et Louis.
vœux(YOHAN♂  Lou♀ CHARLOTTE♀ Henry♂  JOHANA♀ ALBERT♂) -> Bonne année, Lou et Henry. ET BONNE ANNÉE JOHANA ALBERT ET PHILLIPE! 
```

