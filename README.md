# Reader de Hors-Champ

Ce projet est le *reader* du journal Hors-Champ. C'est une plateforme de publication et de lecture des articles du journal.

Le *reader* fonctionne grâce au générateur de site internet statique [Hexo](https://hexo.io).

#### Liens utiles
- Le [framapad](https://mensuel.framapad.org/p/30isjvekmk-9hv2?lang=fr)
- La [feuille de triche](https://github.com/wizhou/hors-champs/wiki/Feuille-de-triche---Markdown) du Markdown
- Le [reader](https://wizhou.github.io/hors-champs/)

## Premiers pas

Pour commencer à travailler, vous devez savoir que :

+ Les articles se trouvent dans le dossier `source`.
+ Le dossier `about` concerne la page __À propos__.
+ Le dossier `_posts` contient l'ensemble des articles du reader.

Chaque article correspond à un fichier au format **Markdown**, comme ceci : `mon-article.md`. Ce fichier contient le texte de l'article et des informations complémentaires.

À chaque article peut être associé un dossier avec des médias, qui doit posséder le même nom que le fichier de l'article. Par exemple `post/mon-article/…`. Les images de l'article sont placées dans ce fichier.

Voici un schéma de l'organisation.

~~~~
_posts/ (le dossier de tous les articles)
├── mon-article.md (le fichier Markdown de l'article)
└── mon-article/ (le dossier médias de l'article)
    └── mon-image.jpg (une image pour l'article)
~~~~

### Créer un un nouvel article

Rendez-vous dans le dossier `source/_posts`, et créer un nouveau fichier. Donner un nom reconnaissable à votre fichier, par exemple `mon-super-article.md`. Le fichier doit être sous l'extention **Markdown**, aisni `.md`. Vous pouvez ensuite commencer à écrire votre article.

### Modifier les informations de l'article

Les informations de l'article sont contenues dans une section spéciale du fichier Markdown appellée **Frontmatter**. Cette section commence avec une ligne de trois tirets `---` et se termine par la même ligne. Chaque article possède cette section.

Voici un exemple de base du *Frontmatter* :
~~~~
---
title: Le titre au propre de l'article
date: la date de publication au format YYYY-MM-DD
type: Le type de l'article (Article | Entretient | Humeur)
author: L'auteurice de l'article.
real: Le ou la ou les réalisateurices de l'article.
---
~~~~

Voici un exemple rempli :

~~~~
---
title: La Guerre des centimes
date: 2019-08-20
type: Article
author: Julien Baroghel
real: Nader S. Ayach
---
~~~~

### Suprimmer l'article

Pour supprimer un article, supprimez simplement le fichier Markdown et le dossier média qui lui sont associé.

## Utiliser Github

Pour éditez un article, rendez-vous sur la page de l'article et cliquez sur le bouton `Edit this file` en forme de crayon. Vous pourrez alors modifier le contenu du fichier.

Une fois vos mofidications terminées, faites un *commit* de celle-ci dans le projet. Pour cela, donner un titre à votre commit, et décrivez simplement ce que vous avez fait, plus cliquez sur le bouton `Commit changes`. Vous verrez deux boutons radio juste au-dessus du bouton commit, ce n'est pas la peine d'y toucher.

## Utiliser Prose

![capture d'écran de Prose](https://raw.githubusercontent.com/wizhou/hors-champs/master/medias/prose.png)

[Prose](prose.io) est un éditeur en ligne qui vous permet de faire des modifications dans vos articles avec un éditeur plus agréable. Pour cela, vous aurez besoin de connectez Prose à votre compte Github, et de lui fournir l'authorisation de faire des modifications pour vous.

Une fois ceci fait, séléectionnez le dossier `hors-champs` et sélectionner l'article sur lequel vous souhaitez travailler dans le dossier `source/_posts`.

- Vous pouvez pré-visualiser vos changements en cliquant sur l'icône `œil`.
- Vous pour éditez les données, ou *frontmatter*, de l'article en cliquant sur le bouton *Meta-Data* avec l'icône `tempalte`.
- Vous pouvez modifier la configurations en cliquant sur le bouon *Settings* avec une icône `rouage`.
- Vous pouvez enregistrer vos changement et faire un *commit* en cliquant sur le bouton *Changes to save* avec une icône `disquette`.


## Travailler ensemble

### Poser des questions

Github propose un outil de gestion d'erreur ou de tâche appelé **Issues**. Si quelque chose vous paraît important, une fonctionnalité semble manquer ou si vous avez besoin d'aide sur quelque chose, n'hésitez pas à créer une nouvelle **Issue** qui représente votre problème !


### Changer les informations

Pour tout ce qui concerne le travail collaboratif, le reader possède un wiki que vous pouvez éditez et modifier à votre guise ! N'hésitez pas à l'utiliser pour poster des informations et alléger le Pad.

En outre, libre à vous d'apportez des modifications aux autres pages d'informations du Reader, comme celle-ci !
