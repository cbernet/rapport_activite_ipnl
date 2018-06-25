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

You can see your commit by doing: 

