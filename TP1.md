TP1

**Exercice 2 : Manuel**

1.  **A l'aide du manuel, identifiez le rôle de la commande which**

> La commande which permet de renvoyer les noms de chemin des fichiers
> exécutables dans l'environnement courant, si ses arguments avaient été
> donnés sous forme de commandes dans un shell strictement conforme à
> POSIX. Il le fait en cherchant l'exécutable dans le PATH.
>
> ![](images/image1.png){width="6.3in"
> height="0.5048611111111111in"}

2.  **Quand on consulte une page du manuel, comment peut-on rechercher
    un terme (par exemple, chercher le terme option dans la page de
    manuel de which ?**

> which --a
>
> ![](images/image2.png){width="5.198641732283464in"
> height="0.5209055118110236in"}

3.  **Comment quitte-t-on le manuel ?**

> En tapant sur la touche « q » du clavier

4.  **Chaque section du manuel a une première page, qui présente le
    contenu de la section. Afficher la première page de la section 6 ;
    de quoi parle cette section ?**

![](images/image3.png){width="6.3in"
height="1.0965277777777778in"}

Cette section parle des jeux et des petits programmes amusants
disponibles sur le système.

**Exercice 3 : Navigation dans l'arborescence des fichiers**

1.  **allez dans le dossier /var/log**

![](images/image4.png){width="3.776127515310586in"
height="0.84375in"}

2.  **remontez dans le dossier parent (/var) en utilisant un chemin
    relatif**

![](images/image5.png){width="3.8026268591426073in"
height="0.53125in"}

3.  **retournez dans le dossier personnel**

![](images/image6.png){width="3.5838331146106737in"
height="0.729268372703412in"}

4.  **revenez au dossier précédent (/var) sans utiliser de
    chemin**![](images/image7.png){width="6.3in"
    height="1.7048611111111112in"}

5.  **essayez d'accéder au dossier /root ; que se passe-t-il ?**

![](images/image8.png){width="5.980001093613298in"
height="1.2918471128608924in"}

Je n'ai pas la permission d'accéder au dossier /rout

6.  **essayez la commande sudo cd /root ; que se passe-t-il ?
    Expliquez**

![](images/image9.png){width="5.5in"
height="0.9348545494313211in"}

cd est une commande shell intégré, sudo ne fonctionne que avec des
exécutables. cd n'est pas une commande qui se trouve dans
/usr/bin:/bin:/sbin/...

7.  **à partir de votre dossier personnel, créez l'arborescence suivante
    :**![](images/image10.png){width="4.959025590551181in"
    height="2.906655730533683in"}

8.  **revenez dans votre dossier personnel ; à l'aide de la commande rm,
    essayez de supprimer Fichier1, puis Dossier1 ; que se passe-t-il ?**

![](images/image11.png){width="3.9067957130358706in"
height="1.4793733595800524in"}

A l'aide de la commande rm le Fichier1.txt a été supprimé mais le
dossier Dossier1 ne peut pas être supprimé.

9.  **quelle commande permet de supprimer un dossier ?**

![](images/image12.png){width="3.2031244531933507in"
height="0.48861220472440947in"}

Pour supprimer un dossier vide il faut utiliser la commande rmdir suivie
le nom du dossier

10. **que se passe-t-il quand on applique cette commande à Dossier2 ?**

![](images/image13.png){width="4.539536307961505in"
height="0.5260411198600174in"}

La commande rmdir ne peut pas supprimer un dossier qui n'est pas vide

11. **comment supprimer en une seule commande Dossier2 et son contenu
    ?**

![](images/image14.png){width="3.675in"
height="1.1666666666666667in"}

La commande rm -r permet de supprimer Dossier2 et son contenu

**Commandes importantes**

1.  **Quelle commande permet d'afficher l'heure ? A quoi sert la
    commande time ?**

**La commande pour afficher l'heure est « date »**

![](images/image15.png){width="2.8337292213473315in"
height="0.6146686351706037in"}

**La commande time permet de déterminer le temps d'exécution d'une
certaine commande.**

![](images/image16.png){width="2.906655730533683in"
height="1.1147386264216972in"}

2.  **Dans votre dossier personnel, tapez successivement les commandes
    ls puis la ; que peut-on en déduire sur les fichiers commençant par
    un point ?**

![](images/image17.png){width="6.3in"
height="0.6951388888888889in"}

Les fichiers commençant par un point sont des fichiers cachés

3.  **Où se situe le programme ls ?**

La programme ls se situe dans /usr/bin/

4.  **Essayez la commande ll. Existe-t-il une entrée de manuel pour
    cette commande ? Utilisez les commandes alias ou alias pour en
    savoir plus sur la nature de cette commande.**

![](images/image18.png){width="2.958746719160105in"
height="0.5834142607174103in"}

Il n'existe pas d'entrée manuel pour cette commande.

![](images/image19.png){width="3.1462718722659666in"
height="0.5834142607174103in"}

Donc la commande ll a été créé manuellement pour remplacer la commande
ls --alF

5.  **Quelle commande permet d'afficher les fichiers contenus dans le
    dossier /bin ?**

Pour afficher les fichiers contenus dans le dossier /bin il faut
utiliser la commande « ls /usr/bin/»

6.  **Que fait la commande ls .. ?**

La commande ls .. permet de lister les fichiers contenus dans le
répertoire parent.

7.  **Quelle commande donne le chemin complet du dossier courant ?**

La commande  « pwd » donne le chemin complet du dossier courant

8.  **Que fait la commande echo \'bip\' \> plop exécutée 2 fois ?**

Cette commande permet de créer un fichier plop en écrivant le texte bip
en une seule ligne si on exécute le fichier 2 fois.

![](images/image20.png){width="3.5629975940507435in"
height="1.1251574803149607in"}

9.  **Que fait la commande echo \'bip\' \>\> plop exécutée 2 fois ?**

![](images/image21.png){width="3.802613735783027in"
height="1.2605927384076991in"}

Cette commande permet de créer un fichier plop en écrivant le texte bip
en deux ligne si on exécute le fichier 2 fois.

10. **Interprétez le comportement de la commande sleep 10 \| echo
    \'toto\' ?**

Cette commande permet d'afficher 'toto' pendant 10 seconde.

11. **A quoi sert la commande file ? Essayez-la sur des fichiers de
    types différents.**

La commande file permet de déterminer le type de fichier indépendamment
de son extension.

![](images/image22.png){width="2.6168930446194225in"
height="0.7417311898512686in"}

12. **Créez un fichier *original* qui contient la chaîne *Hello* *Toto*
    ! ; créer ensuite un lien *lien_phy* vers ce fichier avec la
    commande *ln* *original* *lien_phy*. Modifiez à présent le contenu
    de *original* et affichez le contenu de *lien_phy* : qu'observe-t-on
    ? Supprimez le fichier *original* ; quelle conséquence cela a-t-il
    sur *lien_phy* ?**

![](images/image23.png){width="2.333744531933508in"
height="2.182292213473316in"}

En modifiant le contenu de **original,** le contenu de **lien_phy** est
modifié également, donc dans les deux fichiers il y a le même contenu.

![](images/image24.png){width="2.2668635170603673in"
height="0.5583814523184601in"}

En supprimant le fichier **original,** le contenu de **lien_phy** n'a
pas été modifié et est accessible**.**

13. **Créez à présent un lien symbolique *lien_sym* sur *lien_phy* avec
    la commande *ln -s lien_phy* *lien_sym*. Modifiez le contenu de
    *lien_phy* ; quelle conséquence pour *lien_sym* ? Et inversement ?
    Supprimez le fichier *lien_phy* ; quelle conséquence cela a-t-il sur
    *lien_sym* ?**

> En modifiant le contenu de **lien_phy**, le contenu de **lien_sym** a
> également été modifié, et inversement en modifiant le contenu de
> **lien_sym**, le contenu de **lien_phy** a été modifié.
>
> Si on supprime le fichier **lien_phy**, le fichier **lien_sym**
> devient introuvable et inaccessible.

![](images/image25.png){width="3.025262467191601in"
height="3.4169630358705163in"}

14. **Affichez à l'écran le fichier /var/log/syslog. Quels raccourcis
    clavier permettent d'interrompre et reprendre le défilement à
    l'écran ?**

« CTRL + S » permet d'interrompre et « CTRL + Q » permet de reprendre le
défilement à l'écran.

15. **Affichez les 5 premières lignes du fichier /var/log/syslog, puis
    les 15 dernières, puis seulement les lignes 10 à 20.**

![](images/image26.png){width="6.3in"
height="4.006944444444445in"}

Affichez les 5 premières lignes du fichier /var/log/syslog : head --5
/var/log/syslog 

Affichez les 15 dernières lignes : tail -15 /var/log/syslog

Afficher seulement les lignes 10 à 20 : head --20 /var/log/syslog \|
tail +10

16. **Que fait la commande dmesg \| less ?**

La commande dmesg \| less permet d'examiner ou contrôler le tampon
circulaire du noyau.

17. **Affichez à l'écran le fichier /etc/passwd ; que contient-il ?
    Quelle commande permet d'afficher la page de manuel de ce fichier
    ?**

Le fichier /etc/passwd contient toutes les informations relatives aux
utilisateurs (login, mots de passe, ...). Pour afficher la page de
manuel de ce fichier il faut utiliser la commande « less /etc/passwd ».

18. **Affichez seulement la première colonne triée par ordre
    alphabétique inverse**

![](images/image27.png){width="3.942007874015748in"
height="4.858754374453193in"}

cut -d \':\' -f 1 /etc/passwd \| sort -r

19. **Quelle commande nous donne le nombre d'utilisateurs ayant un
    compte sur cette machine (pas seulement les utilisateurs
    connectés)**

![](images/image28.png){width="3.0919346019247596in"
height="0.6000524934383202in"}

cat /etc/passwd \| wc -l

20. **Combien de pages de manuel comportent le mot-clé conversion dans
    leur description ?**

![](images/image29.png){width="3.058597987751531in"
height="0.49170931758530184in"}

man -k conversion \| wc -l

21. **A l'aide de la commande find, recherchez tous les fichiers se
    nommant passwd présents sur la machine.**

![](images/image30.png){width="4.5587281277340335in"
height="2.5668886701662292in"}

sudo find / -type f -name passwd

22. Modifiez la commande précédente pour que la liste des fichiers
    trouvés soit enregistrée dans le fichier \~/list_passwd_files.txt et
    que les erreurs soient redirigées vers le fichier spécial /dev/null

23. Dans votre dossier personnel, utilisez la commande grep pour
    chercher où est défini l'alias ll vu précédemment.

L'allias ll est défini dans le fichier caché .bashrc à la ligne 91.

![](images/image32.png){width="2.8335793963254594in"
height="0.49170931758530184in"}

24. Utilisez la commande locate pour trouver le fichier history.log.

![](images/image31.png){width="2.8335793963254594in"
height="0.49170931758530184in"}

25. Créer un fichier dans votre dossier personnel puis utilisez locate
    pour le trouver. Apparaît-il ? Pourquoi ?

**Exercice 3 : Travailler avec plusieurs shells**

1.  cp /var/log/syslog /home/User

cp syslog log.txt

nano log.txt

2.  CTRL + W, CTRL + R, chercher le mot kernel + ENTRER, mettre le mot
    noyau + ENTRER, A pour remplacer toutes les occurrences.

3.  CTRL + K pour couper, CTRL + U pour copier

4.  CTRL + U pour annuler

5.  CTRL + S pour enregistrer, CTRL + X quitter nano

Exercice 4 : Personnalisation du shell

![](images/image33.png){width="2.8335793963254594in"
height="0.49170931758530184in"}