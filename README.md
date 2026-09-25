# Jeux_Linux

1° - Faites un Fork de ce Repository GitHUb. Si besoin, voici une vidéo d'accompagnement pour vous aider à "Forker" un Repository Github : https://www.youtube.com/watch?v=p33-7XQ29zQ

2° - Lancer Codespace : Bouton [CODE] puis [Codespace]

3° - Dans le terminal de votre Codespace collez une à une les lignes de commande suivantes :

//Ligne 1 à copier dans le terminal
```C
docker container run -ti ubuntu:18.04 bash
```
//Ligne 2 à copier dans l'instance du laboratoire
```C
apt-get update && apt-get install -y psmisc nano tree xdotool xinput ldap-utils wget bsdmainutils gcc git python3
```
//Ligne 3
```C
git clone https://github.com/bstocker/gameshell.git && cd gameshell
```
//Ligne 4
```C
tar -xvf GameShell.tgz
```
//Ligne 5
```C
echo "true" > ./GameShell/missions/17_bg/check.sh
```
//Ligne 6
```C
./GameShell/start.sh
```
//Ligne 7
```C
PYTHONIOENCODING=utf-8 LC_ALL=C.UTF-8 gash restart
```

4° - -----------------------------------------
Lorsque vous verrez #Mission[1], vous devrez alors utiliser les commandes suivantes :

gash show -> Pour découvrir l'objectif de votre mission

gash check -> Pour demander la validation de votre mission


5° - -----------------------------------------
Solutions pour quelques missions difficiles :

#Mission[3]
```
cd
cd Chateau/Batiment_principal/Salle_du_trone/
gash check
```

#Mission[17]
gash check

#Mission[18]
Faire tree
