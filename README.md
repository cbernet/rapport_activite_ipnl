# Rapport d'activité IPNL/CMS

From now on, the rapport d'activité is written in markdown, which is also used for the [present README](https://raw.githubusercontent.com/cbernet/rapport_activite_ipnl/master/README.md). Here is [some information about markdown](https://fr.wikipedia.org/wiki/Markdown). 

## Prerequisites

* [set up git](https://help.github.com/articles/set-up-git/)
* have at least very basic knowledge about Git. If you don't, look at [follow this simple guide](http://rogerdudler.github.io/git-guide/) and contact Colin in case of problems.
* a text editor. You could use emacs or any other text editor you're familiar with, but you will get a much better experience from an editor that can interpret your text as you type, so that you can see what you're doing. 
	* [MacDown](https://macdown.uranusjr.com/) on the mac
	* [Atom](https://atom.io/) on windows or linux

## Prepare your working directory

* Click on Clone or Download at the top right
* Copy the address starting with https, and do:  

```
git clone git@github.com:cbernet/rapport_activite_ipnl.git
cd rapport_activite_ipnl
```

This clones my repository, and you end up with a local repository that belongs to you.
The clone operation initializes your local repository automatically, no need to do `git init`, as you may have seen is the [simple guide](http://rogerdudler.github.io/git-guide/) provided above. 


## Create your first document

From now on, the rapport d'activité is written in markdown, which is also used for the [present README](https://raw.githubusercontent.com/cbernet/rapport_activite_ipnl/master/README.md). Here is [some information about markdown](https://fr.wikipedia.org/wiki/Markdown). 

To create your document, do e.g. : 

```
touch higgs_gamma_gamma.md
```
and open this file with your editor. 

write a few lines, and then commit to your local repository: 

```
git commit -am 'initial version of the higgs to gamma gamma section'
```

Your commit has been registered to your local repository, and has not yet been shared with us. For now, it remains private to you. 

You can see the commits in your repository by doing: 

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

Now select the commit id (the long hexadecimal number) of one of the commits, or at least the first part of the number, and do: 
```
git show 9f371d7b
```

Commit often as you write (I decide to commit when I'm done with the outline, or with a paragraph).

## Guidelines 

### Initial mail from Raphaël

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
	- introduction: Colin (1/2 page)
	- objets: Colin / Viola (1 page)
	- H->gamma gamma: Suzanne (1 page)
	- H->tau tau: Colin (1 page)
	- ttH: Nicolas (1 page) 
	- HH: Maxime (1 page)
	- Exo: Maxime (1 page)
- upgrade: 
	- introduction: Maxime (1/2 page)
	- upgrade tracker: Seb / Nicolas (3 pages) 
	- upgrade mu-RPC (Imad)

### Recommendations 

**Merci de vous tenir à la limite indiquée ci-dessus, qui constitue une limite dure. Idéalement, essayez de faire moins long. 1 page correspond à environ 500 caractères et 1 ou deux figures.**

**Prenez bien en compte la présence de sections d'introduction.** Par exemple, la question de Higgs additionels et la nécessité de mesurer précisément les couplages de Yukawa ou lambda seront abordées dans la section d'introduction générale.

Mettez vos figures dans un sous-répertoire du répertoire [Figures](Figures).

Les références sont directement insérées comme un lien vers un document public, comme par exemple [particle-flow reconstruction](https://arxiv.org/abs/1706.04965).

Utilisez toujours votre spell-checker avant de partager vos documents


## Examples

* [cms_hub.md](cms_hub.md) Main CMS section
* [upgrade_tracker.md](upgrade_tracker.md) Upgrade tracker section


## Partager votre travail

