# Guide d'utilisation de Markdown#

### Informations utiles et outils###

Pour découvrir Markdown et voir un peu ce qu’il peut faire, vous pouvez essayer un des nombreux éditeurs en ligne comme [markable](https://markable.in/accounts/login/?next=/editor/), l’éditeur original de Gruber, [dingus](https://daringfireball.net/projects/markdown/dingus) ou encore le très puissant [stack edit](https://stackedit.io/) que vous pouvez synchroniser avec Google docs.

Il existe de nombreux éditeurs offlines. **Byword** est une bonne application; *Mac Os, payant*. Pour *Windows*, il existe **Write Monkey**, un peu austère à mon goût, mais très fonctionnel et *gratuit*. Pour *Windows* également, **Markdown Pad 2**, **Typora**, **Caret**, **Texts**, **Atom** et **Haroopad** *gratuits*. Pour *Linux*, il existe **ReText**.

Il reste possible d’ouvrir et d’éditer des fichiers Markdown avec n’importe quel éditeur de code ou éditeur textuel (le **Notepad** ou le **Textedit** livré avec votre système d’exploitation). Mais vous êtes alors privé de la coloration syntaxique et de la prévisualisation en temps réel de ce que vous êtes en train d’écrire.

Dans notre cas **MarkdownPad 2**, **Typora** et **Atom** sont les seuls logiciels utilisables pour le moment. Bien que le premier soit plus adapté à une utilisation débutante de Markdown grâce à son double affichage (code et visuel rendu), le second est à mon sens plus agréable étant donné son design épuré et le choix plus important de possibilités. Pour ce qui est du troisième il fait un mélange entre les deux et il semblerait qu’il se prêtera plus à l’utilisation du GIT. Il revient donc à chacun de choisir celui qui lui conviendrait le mieux. 

PS : Pour obtenir le double affichage sur **Atom** il suffit de faire un « *Ctrl+Shift+M* » ou « *Packages>Markdown Preview>Toggle Preview* ». Egalement sur **Atom**, pensez à enregistrer le fichier en .md, au moins au début, pour pouvoir bénéficier de toutes les possibilités disponibles.

Beaucoup d’autres possibilités d’utilisation de Markdown existent grâce à l’ajout de Pandoc mais le serveur Proxy empêche le téléchargement de ce complément.



###La syntaxe de Markdown###

#####Les titres#####

Il est possible de titrer en ajoutant des dièses au début de la ligne. Il n’y a pas de limite au nombre de niveaux de titres qu’il est possible d’utiliser (mais n’allez pas au-delà de 7).

![1](ScreenShots/1.png)



Il existe une autre façon de titrer mais uniquement pour les deux premiers niveaux. Pour le premier niveau il faut mettre au moins un ` = ` sur la ligne en dessous du titre et pour le deuxième niveau au moins un ` - ` sur la ligne en dessous :



![2](ScreenShots/2.png)



#####Les paragraphes#####

Pour afficher un paragraphe, sautez deux ligne et de taper son texte. Un seul saut de ligne correspond à un
retour chariot et pas à un changement de paragraphe.



![3](ScreenShots/3.png)



#####Les sauts de ligne simples#####

Effectuer un saut de ligne simple dans votre texte Markdown n’aura aucun effet sur l’Export HTML, sauf si vous terminez votre ligne par un double espace (ou plus que ça). Un retour chariot sera alors exporté.





![4](ScreenShots/4.png)

![5](ScreenShots/5.png)



#####L'emphase#####

Pour faire de l'emphase, c'est-à-dire de la mise en valeur, il vous suffit d'entourer les mots de votre choix entre des étoiles `*` ou des traits de soulignement `_` (au choix, le résultat est le même).

###### Faible######

Elle sert à mettre un mot ou une phrase en *Italique*.

![6](ScreenShots/6.png)




###### Forte######

Elle sert à mettre un mot ou une phrase en **Gras**.

![7](ScreenShots/7.png)



On peut bien entendu combiner les deux types d’emphase.

![8](ScreenShots/8.png)



#####Barrer un mot#####
Pour barrer un mot ou une phrase en Markdown il faut normalement entourer le mot ou la phrase voulu par deux `~`. Mais cette option n’est pas disponible avec tous les logiciels. Ainsi, sur Typora/Atom on pourra utiliser le  `~`, par contre sur MarkdownPad 2  il faudra se servir des balises HTML.



![9](ScreenShots/9.png)

![10](ScreenShots/10.png)

![11](ScreenShots/11.png)




#####Les citations#####
Pour afficher un bloc de citation, commencez le paragraphe par un chevron fermant. Si votre bloc contient plusieurs lignes, vous pouvez faire des sauts de lignes à la main et toutes les ouvrir par un chevron fermant, mais ce n’est pas nécessaire. Ces blocs peuvent contenir d’autres éléments Markdown comme des titres ou des listes.

![12](ScreenShots/12.png)




#####Les listes non ordonnées#####
Pour afficher une liste, commencez la ligne par un astérisque `*`, un moins `-` ou un plus `+`. Le choix n’a pas d’importance, mais il faut rester cohérent dans votre document. Il faut faire attention à mettre un espace entre le `-/+/*` et le début du mot ou de la phrase.

![13](ScreenShots/13.png)




#####Les listes ordonnées#####
Pour afficher une liste ordonnée, commencez la ligne par un nombre suivit d’un point. 

![14](ScreenShots/14.png)



Il n’est pas nécessaire de mettre le bon numéro de point de la liste pour toutes les lignes si le premier point a été déclaré correctement :

![15](ScreenShots/15.png)



######Les sous-parties######
Il est possible d’ajouter des sous niveaux dans les listes  (non ordonnées et ordonnées). Pour cela, il suffit d’ajouter une tabulation avant les sous-points :

![16](ScreenShots/16.png)

![17](ScreenShots/17.png)




#####Les Checklist#####
Utilisez `[ ] ` ou ` [x] ` pour faire une checklist. Vous devez précéder la checklist avec soit ` -<espace> `, soit  ` 1.<espace> ` (ou n’importe quel nombre).

![18](ScreenShots/18.png)



Pour modifier les cases qui sont censées être cochées il ne suffit pas de cliquer dans les cases. Il faut bien entendu changer le code, car même en enregistrant cela ne changerait rien.

Cette fonction n’est pas disponible sur MarkdownPad 2 mais existe sur Typora/Atom.


#####Le bloc de code#####
Pour afficher un bloc de code, sautez deux lignes comme pour un paragraphe, puis indentez avec 4 espaces ou une tabulation. Le bloc se terminera dès qu’il arrivera sur une ligne non indentée.

![19](ScreenShots/19.png)




#####Le code en ligne#####
Pour afficher du code dans une ligne, il faut l’entourer par des guillemets simples : *`<Altgr+7>`*.

![20](ScreenShots/20.png)




#####Les filets ou barres de séparation#####
Pour afficher un filet/barre de séparation il suffit d’entrer au moins trois astérisques `*` ou moins `–` (il n’y a pas de différence entre les deux) sur une ligne entourée de sauts de lignes. Restez juste cohérent dans votre document.

![21](ScreenShots/21.png)




#####Les liens#####
Il y a deux façons d’afficher un lien. De manière automatique en encadrant un lien par des chevrons. Il est alors cliquable et affiche l’url indiquée entre chevrons. Ou en ajoutant des paramètres. Le texte à afficher est alors indiqué entre crochets suivit de l’adresse du lien entre parenthèses, ce texte sera affiché à la place du lien, ce qui est plus esthétique. Dans les parenthèses, à la suite du lien, on peut indiquer un titre entre guillemets. Ce titre sera affiché lors du survol du lien dans le navigateur.

![22](ScreenShots/22.png)



Utilisation de liens par référence dans un texte 

![23](ScreenShots/23.png)



L’insertion d’une adresse email se fait de la même façon que pour insérer un lien, il est tout de même recommandé de rajouter ` mailto: ` avant l’adresse.



#####Les images#####
Pour afficher une image, commencez par un point d’exclamation. Puis indiquez le texte alternatif entre crochets. Ce dernier sera affiché si l’image n’est pas chargée et lue par les moteurs de recherche. Terminez par l’URL de l’image entre parenthèses. Après le lien vers l’image, il est possible d’ajouter un titre lu par les navigateurs textuels et affiché au survol de l’image par les autres.

![24](ScreenShots/24.png)



ATTENTION : Sur MarkdownPad 2, avant d’afficher l’image, le logiciel va vous demander de vous connecter. Les identifiants de connexion sont ceux de votre compte utilisateur.

Il est également possible d’utiliser un chemin local pour charger l’image mais cette fonction n’est pas disponible sur MarkdownPad 2/Atom. Elle fonctionne en revanche très bien sur Typora.

![25](ScreenShots/25.png)



#####Lien et image#####
Lorsqu’on veut insérer un lien dans le document tout en mettant le logo et donc combiner les deux c’est possible et pratique avec Markdown.

![26](ScreenShots/26.png)



Il existe aussi la méthode du « Drag & Drop » pour insérer des images, des liens ou encore des documents externes (il faut pour ces derniers installer le plugin Pandoc qui est bloqué sur nos ordinateurs par le Proxy). Pour cela il suffit de sélectionné le fichier/lien souhaité et le déposer en le faisant glisser dans le code Markdown, le logiciel que vous utilisez s’occupera d’insérer automatiquement le code correspondant. Cette fonction n’est vraiment utilisable que sur Typora. Voici les types de fichiers normalement supportés :
- Images : PNG (.png), GIF (.gif), JPEG (.jpeg & .jpg) 
- Documents : Word (.docx), Excel (.xlsx), Powerpoint (.pptx), fichiers textes (.txt), PDFs (.pdf) 
- Fichiers compressés : ZIP (.zip), GZIP (.gz) 
- Fichiers vidéo : MOV (.mov), MP4 (.mp4)




#####Les tableaux#####
L’idée globale est de "dessiner" des colonnes en les entourant avec des pipes `|`. Le nombre de colonnes est défini dans la première ligne du tableau et vous devez pour chaque ligne avoir le même nombre de colonnes, même si certaines sont vides.
La première ligne sera votre en-tête. La seconde ligne sépare cet en-tête du corps du tableau et définit l’alignement du texte dans les colonnes. Elle ne contient que des tirets - et des deux points : sont utilisés pour définir cet alignement. Pas de : ou juste un à gauche signifie que le texte sera aligné à gauche. Si la ligne de ` -` est entourée de 2 ` :` le texte sera centré et si un seul : est présent à droite de la ligne, le texte sera aligné à droite.
Cette option n’est pas disponible sur MarkdownPad 2 mais présente sur Typora/Atom, par contre il faut d’abord passer en mode code source : *` View>Source Code Mode`* ou *`Ctrl + : `* ou (en bas à gauche de la fenètre) *` </> Toggle Source Code Mode`*.

![27](ScreenShots/27.png)

![27-2](ScreenShots/27-2.png)




#####Les notes de bas de page#####
En Markdown il est possible d’insérer des notes de bas de page. Encore une fois MardownPad 2 va poser problème car la quantité d’information que l’on donner à la note est très limitée, alors que Typora/Atom ne limite pas.

![28](ScreenShots/28.png)

![29](ScreenShots/29.png)




#####Les emojis#####
Sur certains logiciels de Markdown il est possible de rajouter des emojis dans le texte. Il faut insérer le texte correspondant à l’emojis entre ` : `. Parmi les emojis on peut retrouver bien sur les smileys mais aussi beaucoup d’autres symboles. Malheureusement, ces symboles n’ont pas tous le rendu espéré étant donné que le logiciel est en noir et blanc.

![30](ScreenShots/30.png)

![31](ScreenShots/31.png)



Parmi les logiciels que j’utilise pour vous faire ce guide, le seul qui supporte ces emojis est Typora. Pour avoir un aperçu des emojis disponibles il suffit de taper un ` : ` suivi d’une lettre. Mais pour cela il ne faut pas être en *` Source Code Mode `*.

![32](ScreenShots/32.png)



###Echappement des caractères###
Les caractères spéciaux ayant un sens en HTML et en Markdown doivent être échappés. Pour les esperluettes `&amp;`, chevrons `<` et autres caractères HTML, Markdown se charge de les convertir en entités HTML lors de l’export. Mais si vous souhaitez utiliser dans votre texte des astérisques, accolades, dièses… à une position indiquant à Markdown que vous désirez un formatage particulier, vous devez les échapper en les faisant précéder d’un antislash \. Sinon Markdown les masquera et appliquera le formatage correspondant. Les caractères suivants sont à échapper :



![33](ScreenShots/33.PNG)

![34](ScreenShots/34.PNG)




###Séparer des blocs###
Une petite chose peut se révéler agaçante : deux blocs consécutifs qui se voient fusionnés. Ce sera le cas de deux blocs de citation ou de code par exemple. Et ce quel que soit le nombre de lignes que vous sauterez. Une solution simple est d’ajouter des commentaires html entre deux blocs. La syntaxe des commentaires est la suivante : `<!-- texte en commentaire -->`. Le texte sera ignoré par le navigateur. Votre commentaire peut tout à fait être vide.



![35](ScreenShots/35.png)

![36](ScreenShots/36.png)




###Engeristrement des documents###
Lors de l’enregistrement d’un document écrit en Markdown sur l’un des deux logiciels utilisé, le format par défaut sera `.md`, c’est-à-dire en Markdown. Afin d’effectuer un enregistrement en HTML il ne faut pas faire un simple enregistrement et changer le format en `.html`, il faut passer par une exportation du fichier vers HTML.
Sur Typora :

*`File>Export>HTML`*


Sur MarkdownPad 2 :

*`File>Export>Export HTML`* ou *`Ctrl+Shift+1`*



###Insertion de langage HTML###
En Markdown il est possible d’utiliser le langage HTML et donc d’insérer des balises HTML dans le document que vous êtes en train d’écrire. Il est à noter cependant que lorsque vous écrivez en HTML dans le texte il n’est pas possible d’utiliser en même temps le Markdown, il faut que la partie HTML soit fermée avant de pouvoir reprendre le Markdown. Voici un petit exemple pour illustrer cela :



![37](ScreenShots/37.png)




###Besoin d'aide?###
Pour ceux qui aurait du mal à comprendre après la lecture de ce guide pas de soucis voici un lien vers un petit tutoriel qui permet d’apprendre les bases du Markdown une étape à la fois en étant bien guidé. Attention, c’est un tutoriel en anglais donc pour ceux qui ne seraient pas à l’aise munissez-vous d’un dictionnaire.
[Tutoriel Markdown](https://www.markdowntutorial.com/)


###Pour aller plus loin###
En plus du Markdown il existe le RMarkdown qui est beaucoup plus complet et possède une quantité bien plus importante de possibilités. Il est possible d’écrire en Markdown simple dans un logiciel de RMarkdown, le rendu sera le même. Le R Markdown est cependant beaucoup plus complexe à apprendre, je laisse donc à chacun la liberté de l’apprendre.
Pour utiliser le RMarkdown je vous conseille RStudio (en anglais) et vous dirige vers cette vidéo pour en apprendre les bases : [Ecrire en RMarkdown avec RStudio](https://www.youtube.com/watch?v=DNS7i2m4sB0)


