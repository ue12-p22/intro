---
jupytext:
  cell_metadata_filter: all,-hidden,-heading_collapsed,-run_control,-trusted
  notebook_metadata_filter: all, -jupytext.text_representation.jupytext_version, -jupytext.text_representation.format_version,
    -language_info.version, -language_info.codemirror_mode.version, -language_info.codemirror_mode,
    -language_info.file_extension, -language_info.mimetype, -toc
  text_representation:
    extension: .md
    format_name: myst
kernelspec:
  display_name: Python 3 (ipykernel)
  language: python
  name: python3
language_info:
  name: python
  nbconvert_exporter: python
  pygments_lexer: ipython3
nbhosting:
  title: introduction
---

Licence CC BY-NC-ND, Thierry Parmentelat & Valérie Roy

```{code-cell} ipython3
:tags: [raises-exception]

%%python
from IPython.display import HTML
HTML(url="https://raw.githubusercontent.com/ue12-p22/intro/main/notebooks/_static/style.html")
```

# introduction

bienvenue dans ce premier cours d'informatique

+++

## objectifs globaux

+++

l'approche pédagogique des cours d'info vise en premier lieu **à vous mener à l'autonomie** en ce qui
concerne l'utilisation des ressources digitales; c'est pourquoi nous ne sommes **pas en
salle informatique** comme ça a pu se faire à une époque; l'objectif est que vous sachiez
à terme utiliser **uniquement votre ordinateur** pour travailler (ce qui a été très
pratique lors des confinements liés au covid).

+++ {"slideshow": {"slide_type": ""}}

en détail, pour le cours d'informatique de 1ère année :

* prise d'**autonomie**  
  * par rapport à un ordinateur personnel
  * par rapport au numérique et à la programmation
  * focus sur quelques outils (du moment)
* pour les mathématiques, le machine-learning et autres enseignements
  * Python - numpy - pandas - matplotlib  
  * notebooks Jupyter
* workflow de gestion de projets de développement
  * git & github
* approfondissement langage (un au choix)
  * Python
  * C++
* culture informatique
  * notions d'algorithmique et de complexité
  * notions sur les systèmes d'exploitation des ordinateurs (OS)   
  * rudiments de programmation Web
  * rudiments sur programmation parallèle
  * rudiments sur l'utilisation du réseau
* projet informatique
  * en équipe
  * posé par une personne extérieure à l'équipe d'enseignants

+++

## objectifs pour cette introduction

+++

ce cours d'introduction vise à présenter, et à vous faire installer, les outils de base
pour le cours d'informatique; il ne présente **aucune difficulté** mais vous êtes invité·e
malgré tout à le suivre **avec une grande attention** car tous ces éléments sont
**cruciaux pour la suite**

+++

notez que

* le cours est **coopératif**, et pas compétitif  
  ceux qui savent déjà **aident leurs camarades**

* xxx voyez aussi la checklist des compétences requises - [notebook
  `2-98-checklist.md`](https://nbhosting.inria.fr/auditor/notebook/ue12-p21-python-primer/notebooks/2-98-checklist)

* à terminer pour la prochaine fois si nécessaire

+++

## installations

nous verrons pour commencer comment installer notre pile logicielle, à savoir essentiellement

* le terminal - nous utilisons **`bash`**, qui est natif sur les OS linux et MacOS, et qui vient avec le produit `git for windows`
* l'éditeur de code **VS-code** (Visual Studio Code)
* **miniconda** pour **Python** (et les environnements virtuels)
* **Jupyter** pour les notebooks
  * et accessoirement, *markdown* pour la mise en forme du texte,
  * et les formules mathématiques en $\LaTeX$
* **`git`** pour la gestion de versions; c'est un outil super-utile pour le développement, c'est indispensable que vous sachiez l'utiliser

+++

## les supports de cours

le plus souvent, les supports de cours sont fournis **sous forme de notebooks**; ce sont des documents hybrides contenant **du texte** (mis en page grâce à *markdown*) et du **code** directement **exécutable**; on peut également y inclure des équations mathématiques, et des média externes (images, vidéos, sons, ...)

+++

### dépôt git

ces contenus vous sont exposés au travers d'un **dépôt git** (hébergé sur <https://github.com>)

en général il y aura **un dépôt par bloc de cours** (typiquement, un pour cette introduction, un pour le cours Python numérique, un pour votre cours de langage, …)

du côté **github.com**, les cours du premier semestre sont exposés sous une **organisation** (c'est un terme propre à github pour structurer l'espace de noms des dépôts, il y en a plusieurs dizaines de millions...) qui s'appelle `ue12-p22`; ça signifie que vous pouvez retrouver tous les cours à cette adresse

<https://github.com/ue12-p22/>

+++

### les contenus sur votre ordi

une des premières choses que nous apprendrons, ce sera donc 

* comment copier ces contenus sur votre ordinateur, en *clonant* le dépôt depuis github vers votre ordinateur
* comment ensuite lire ces contenus (principalement des notebooks donc) sur votre ordinateur

+++

### `nbhosting`

vous aurez également accès à une plateforme hébergée sur <https://nbhosting.inria.fr>) où ces contenus seront accessibles sans installation préalable; cette facilité est conçue essentiellement pour les premiers cours, de sorte que l'on puisse avancer avant que toute la promo soit entièrement bien installée sur les ordis perso

il devrait être entendu que le mode d'utilisation "normal" des supports est **en local sur votre ordi**, le recours à nbhosting est conçu comme transitoire, et devrait disparaitre progressivement au cours de l'année

+++

### supports HTML cherchables 

la plupart du temps, les contenus notebooks sont également publiés sur *nbhosting* dans un format `HTML`; il s'agit bien sûr d'une version statique (on ne peut plus modifier le code), mais par contre on peut y faire des recherches globalement, ce qui est pratique dans les cours qui contiennent un grand nombre de notebooks
