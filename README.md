# Rapport d'activité IPNL/CMS

Le rapport d'activité est désormais écrit en markdown, ce qui est aussi le cas de ce 
[README](https://raw.githubusercontent.com/cbernet/rapport_activite_ipnl/master/README.md). Voici [quelques informations sur markdown](https://fr.wikipedia.org/wiki/Markdown). 

## Avant toute chose

Il vous faut: 

* [installer git](https://help.github.com/articles/set-up-git/)
* des connaissances basiques sur Git. Si ce n'est pas le cas [suivez ce guide très simple](http://rogerdudler.github.io/git-guide/) et demandez de l'aide à Colin si besoin est.
* un éditeur de texte. Vous pouvez utiliser emacs ou tout autre éditeur de texte dont vous êtes familier. Mais il sera plus confortable d'utiliser un éditeur capable d'interpréter le markdown pendant que vous tapez:
	* [MacDown](https://macdown.uranusjr.com/) sous mac OS
 	* [Atom](https://atom.io/) sous windows ou linux

## Preparer son répertoire de travail

*À ne faire qu'une fois*

* Cliquez sur _Clone or Download_ en haut à droite
* Copiez l'adresse https et tapez ceci dans la ligne de commande:  

```
git clone <adresse>
cd rapport_activite_ipnl
```

Ceci clone ma version du repository, et vous obtenez un repo local qui vous appartient. 
Le clonage initialise le repo local automatiquement, et vous n'avez donc pas à taper `git init` comme vous avez pu le voir dans le [guide](http://rogerdudler.github.io/git-guide/) donné ci-dessus. 


## Créez votre document

Créez un fichier vide 

```
touch higgs_gamma_gamma.md
```

et ouvrez le dans votre éditeur. 

écrivez quelques lignes, et committez dans votre repo local: 

```
git commit -am 'initial version of the higgs to gamma gamma section'
```

Votre commit a été enregistré dans votre repo local, mais n'a pas encore été partagé avec nous. Pour l'instant, vos modifications restent donc privées. 

Vous pouvez voir les commits dans votre repo comme cela: 

```
git log
> 
commit 9f371d7bd606659a56ecbaceeed9339de8a908cb
Author: Colin <colin.bernet@cern.ch>
Date:   Mon Jun 25 15:22:54 2018 +0200

    first explanations

commit c58ffcf1b752c0b316c3b2b98a618d34b24aa156
Author: Colin Bernet <colin.bernet@cern.ch>
Date:   Mon Jun 25 14:59:19 2018 +0200

    Initial commit
```

Maintenant, sélectionnez un commit id (le long nombre hexadécimal) de l'un des commits, ou au moins une partie au début de ce nombre, puis faites: 

```
git show 9f371d7b
```

**Committez souvent!** Personnellement, je commite après avoir avancé dans mon plan détaillé, puis après chaque paragraphe. 

## Organisation 

### Mail initial de Raphaël

En vue de la préparation du dossier HCERES de l’année prochaine, un rapport d’activité de l’unité couvrant les années 2015-2017 est en cours de préparation.
Pour cette édition, nous avons décidé de construire le RA par projet, ceci afin de minimiser les redites au sein du document entre les parties écrites par les équipes de recherche et celles écrites par les services techniques.

Nous nous dirigeons vers un format purement dématérialisé sur le site web du laboratoire, donc a priori nous n’avons pas de contrainte de place. Néanmoins en vue d’utiliser ce rapport d’activité comme input au dossier HCERES et dans une moindre mesure au dossier de renouvellement du Labex LIO, nous vous demandons de limiter le texte à environ 1 à 2 pages par projet auxquelles vous joindrez 1 ou 2 figures/photos pour illustration.

Pour les activités de CMS je vois les contributions suivantes auxquelles j’ai associé un(des) nom(s) de responsable(s) :

- Activités d’analyse de Physique : Roberto, Colin. **Raphaël confirme qu'il souhaite environ une page par projet de physique**
- Projet upgrade Tracker (CIC, Dee, FastTrack) : Sébastien, Luigi, Nick, Nicolas [cette contribution peut-être partagée en plusieurs contributions si vous préférez]
- Projet upgrade Muon-RPC : Imad, Laurent, Christophe

Les différentes parties, en particulier pour les projets, doivent être écrites de telle sorte d’inclure les contributions des services techniques.

Un premier draft de l’ensemble des contributions devra être disponible d’ici à la fin Juin.

### Répartition des tâches

Voici ce que je propose. La discussion est ouverte, contactez-moi directement si vous voyez un souci avec ça:  

- introduction globale : Rob (1/2 page)
- physique: 
	- Introduction: Rob (1/2 page)
	- Objets: 
		- particle flow: Colin (1/2 page, 1 figure)
		- jet energy corrections: Viola (1/2 page, 1 figure)
	- Bosons de Higgs additionnels:
		- H->gamma gamma: Suzanne (1/2 page, 1 figure)
		- H->tau tau: Colin (1/2 page, 1 figure)
		- top: Stéphane, Rob, Viola (1/2 page, 1 figure)
	- Caractérisation du boson de Higgs: 
		- HH: Maxime (1/2 page, 1 figure)
		- ttH: Nicolas (1/4 page, 1 figure)
	- Vector-like quarks: Steph (1/2 page, 1 figure)
- upgrade: 
	- introduction: Maxime (1/2 page, éventuellement 1 figure physique)
	- upgrade tracker: Seb / Nicolas (endcaps, concentrateur, déclenchement, 3 pages, 3 figures) 
	- upgrade mu-RPC: Imad (1 page, 3 figures) 


### Quelques recommendations

#### Limites sur la taille du texte

**Merci de vous tenir à la limite indiquée ci-dessus, qui doit être prise comme une limite dure. Idéalement, essayez de faire moins long. 1 page correspond à environ 500 mots et une ou deux figures.** Vous pouvez compter le nombre de mots d'un fichier en faisant: 

```
wc upgrade_tracker.md
>      14    1801   12712 upgrade_tracker.md
```

Ce fichier fait donc 1801 mots pour l'instant, ce qui est presque bon (en effet, ce projet contient 3 sous-projets, et doit donc être décrit en moins de 1500 caractères). Il contient 11 figures, et il serait donc bien d'en enlever environ la moitié, la limite étant fixée à 6 figures.  

#### Prenez bien en compte la présence de sections d'introduction.

Par exemple, la question de Higgs additionels et la nécessité de mesurer précisément les couplages de Yukawa ou lambda seront abordées dans la section d'introduction générale.

#### Figures

Mettez vos figures dans un sous-répertoire du répertoire [Figures](Figures).
Pour insérer une figure, faire: 

```
![Figures/tracker/dee_3d.png](Figures/tracker/dee_3d.png)

*Fig 3: Vue d'un Dee (chaque disque est composé de quatre Dees)*
```

#### Références

Les références sont directement insérées comme un lien vers un document public, comme par exemple l'article sur la [reconstruction du flux de particules dans CMS](https://arxiv.org/abs/1706.04965).

#### Spell checker 

Utilisez toujours votre spell-checker avant de partager vos documents

#### Formules mathématiques

Elles n'ont sans doute pas lieu d'être dans un tel document. Si vous ne pouvez absolument pas faire sans, mettez votre formule en texte verbatim comme cela: 

```
\eta = -{\rm log} ({\rm tan} \frac{\theta}{2})
```

Je ne sais pas encore comment faire, mais je sais qu'il existe des plugins pour interpréter une formule latex en markdown.

## Examples

* [cms_hub.md](cms_hub.md) Main CMS section
* [upgrade_tracker.md](upgrade_tracker.md) Upgrade tracker section


## Partagez votre travail

Après avoir committé dans votre repo local, celui-ci contient des commits que vous souhaitez partager avec mon repo github.

Pour cela, la procédure est la suivante, nous allons couvrir tous les points en détail par la suite, et vous pouvez trouver plus d'infos [ici](https://help.github.com/articles/fork-a-repo/).

- recupérer les dernier commits de _mon_ repo github (ces commits ont pu être rajoutés par d'autres personnes)
- poussez votre branche master sur _votre_ repo github 
- faire une pull request de _votre_ repo vers _mon_ repo pour me transférer vos changements. 

### Mise en place de votre repo github

*À ne faire qu'une fois*

Pour l'instant, vous avez directement créé votre repo local sur votre ordinateur à partir de mon repo sur github. Nous allons maintenant créer votre propre repo github et le connecter à votre repo local. 

![](Figures/schema_git.pdf)

*Liens entre les repos git. Ce qui se trouve dans la bulle est sur github. Votre repo local est sur votre ordinateur. Pour l'instant, vous vous êtes contentés de cloner mon repo github pour créer votre repo local.*

- allez sur [mon repo github](https://github.com/cbernet/rapport_activite_ipnl)
- cliquez sur **Fork** tout en haut a droite. Cela crée votre repo github, et vous redirige dessus
- cliquez sur **Clone or Download** en haut à droite, et copiez le lien https vers votre repo. 
- allez dans votre répertoire de travail, et faites: 

```
git remote add my-repo <lien_https>
```

Vous pouvez obtenir la liste des repos remote (c'est à dire ceux qui sont connectés à voter repo local) en faisant: 

```
git remote -v
```

Vous devriez voir le mien et le vôtre. 

### Récupération des derniers commits depuis mon repo, 

- récupérer ces commits depuis mon repo

```
git fetch origin 
```
- mélangez ces modifications à votre version locale: 

```
git merge origin/master
```

- assurez-vous que le texte est ok

### Pull request

- poussez vos commits vers votre repo github: 

```
git push my-repo master
```

- allez sur votre repo github grâce à votre navigateur, et faites une pull request vers mon repo github. Les informations pour cela devraient vous être données automatiquement sur la page de votre repo. 


