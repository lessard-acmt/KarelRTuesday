# Karel R Tuesday

Projet pedagogique en **Ruby** concu pour le cours **ICS3U** (Ontario) afin d'aider les eleves a developper leurs competences en programmation, en **programmation orientee objet** et en techniques de resolution de problemes par le code.

Ce projet s'appuie sur l'idee classique de **Karel le Robot**, un environnement d'apprentissage ou un robot execute des commandes simples dans un monde en 2D. L'approche permet aux eleves de se concentrer sur la logique, les algorithmes et la structure du code avant de passer a des projets plus complexes.

Ce depot est inspire du projet original de Joseph Bergin :
**Karel Ruby** - https://csis.pace.edu/~bergin/KarelRuby/

## But pedagogique

Ce projet est utilise en classe pour aider les eleves a :

- apprendre les bases du langage **Ruby**;
- comprendre les principes de la **programmation orientee objet**;
- developper des algorithmes clairs et logiques;
- decomposer un probleme en petites etapes;
- pratiquer le debogage et l'amelioration de code;
- explorer des techniques de programmation comme la reutilisation, l'heritage et l'extension de classes.

## Qui est Karel?

**Karel** est un petit robot programme pour accomplir des taches dans un monde quadrille en 2D.

Son monde est compose de :

- **rues** allant d'est en ouest;
- **avenues** allant du nord au sud;
- **intersections** ou les rues et les avenues se croisent;
- **murs** qui bloquent certains passages;
- **beepers** places sur les intersections;
- parfois d'autres robots presents dans le meme monde.

L'intersection de la **1re rue** et de la **1re avenue** represente l'origine du monde. Karel se deplace d'une intersection a l'autre, une case a la fois.

## Les capacites de Karel

Karel dispose d'un ensemble limite d'actions et de capteurs. Cette simplicite est volontaire: elle pousse les eleves a reflechir a la logique de leurs programmes.

Karel peut notamment :

- avancer d'un bloc a la fois;
- tourner a gauche;
- detecter s'il y a un mur devant lui;
- detecter si un beeper se trouve sur son intersection;
- ramasser des beepers;
- deposer des beepers;
- verifier son orientation (nord, sud, est, ouest);
- detecter si un autre robot se trouve sur la meme intersection;
- s'eteindre lorsque sa tache est terminee.

## Taches et situations

Dans l'univers de Karel, on distingue souvent :

- une **situation** : la description du monde de depart;
- une **tache** : ce que le robot doit accomplir.

Exemples de taches :

- se rendre a une intersection precise;
- contourner des obstacles;
- s'echapper d'une piece avec une porte;
- traverser un labyrinthe;
- ramasser tous les beepers d'un monde.

Cette approche aide les eleves a analyser un probleme, a planifier une solution, puis a coder cette solution de facon structuree.

## Pourquoi utiliser Karel en ICS3U?

Karel est un excellent outil pour introduire plusieurs concepts importants du cours, par exemple :

- les variables et les methodes;
- les structures de controle;
- la decomposition d'un probleme;
- la conception de classes et d'objets;
- la reutilisation de code;
- le test et le debogage.

Comme le monde de Karel est volontairement simple, les eleves peuvent consacrer plus d'energie a la **pensée algorithmique** et a la **qualite de leur code**.

## Structure du depot

Le depot contient notamment les dossiers suivants :

- `karel/` : les classes principales du projet et la logique du robot;
- `mixins/` : du code reutilisable ajoute a certaines classes;
- `tasks/` : des taches ou scenarios a executer;
- `worlds/` : des mondes de depart pour les activites;
- `Gemfile` : les dependances Ruby du projet.

## Installation

### 1. Forker et Cloner le depot

```bash
Fork le depot dans votre compte de Github
Avec Github Desktop, faites un clone de VOTRE copie du depot
cd KarelRTuesday
```

### 2. Installer les dependances

```bash
bundle install
```

## Utilisation

Une execution typique se fait a partir d'un fichier dans le dossier `tasks/`.

Par exemple :

```bash ou Rubymine
ruby tasks/main.rb
```

Selon l'activite choisie, vous pouvez modifier la tache executee ou utiliser d'autres fichiers dans le dossier `tasks/`.

## Exemples d'activites en classe

Voici quelques exemples d'activites possibles avec ce projet :

- guider Karel jusqu'a une destination;
- faire ramasser a Karel tous les beepers d'un monde;
- programmer Karel pour suivre un mur;
- resoudre un petit labyrinthe;
- creer de nouvelles classes de robots avec des comportements specialises;
- comparer plusieurs strategies pour accomplir la meme tache.

## Liens avec la programmation orientee objet

Ce projet permet de montrer concretement que :

- un **robot** peut etre represente comme un **objet**;
- ses actions sont definies par des **methodes**;
- differents types de robots peuvent etre crees a partir d'une classe de base;
- on peut **modifier** ou **etendre** le comportement d'un robot selon les besoins.

Ainsi, Karel sert non seulement a apprendre a coder, mais aussi a comprendre comment organiser du code de maniere claire, modulaire et reutilisable.

## Public cible

Ce projet a ete prepare pour des eleves du cours **ICS3U** selon le cadre du curriculum de l'Ontario, en particulier pour soutenir l'apprentissage de :

- la logique de programmation;
- la conception de solutions;
- la programmation en Ruby;
- la programmation orientee objet;
- les bonnes pratiques de codage.

## Credits

- Adaptation pedagogique pour le cours **ICS3U**
- Inspire du projet original **Karel Ruby** de Joseph Bergin
- Projet original : https://csis.pace.edu/~bergin/KarelRuby/

## Reference

Ce README s'appuie sur la structure publique du depot GitHub et sur la presentation de cours jointe sur Karel et son monde.
