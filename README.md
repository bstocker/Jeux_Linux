# 🐧 Jeux_Linux

Apprenez les commandes Linux en jouant avec un jeu d'aventure dans le terminal.

---

## 🚀 Installation

### 1. Forker le dépôt

Faites un **Fork** de ce repository GitHub.

> 📺 Besoin d'aide ? Voici une vidéo d'accompagnement pour « forker » un repository GitHub :
> https://www.youtube.com/watch?v=p33-7XQ29zQ

### 2. Lancer Codespace

Cliquez sur le bouton **`Code`**, puis sur l'onglet **`Codespaces`**.

### 3. Installer et lancer le jeu

Dans le terminal de votre Codespace, collez **une à une** les lignes de commande suivantes.

**Étape 1** — Lancer un conteneur Ubuntu *(à copier dans le terminal du Codespace)* :

```bash
docker container run -ti ubuntu:18.04 bash
```

**Étape 2** — Installer les dépendances *(à copier dans l'instance du laboratoire)* :

```bash
apt-get update && apt-get install -y psmisc nano tree xdotool xinput ldap-utils wget bsdmainutils gcc git python3
```

**Étape 3** — Cloner GameShell :

```bash
git clone https://github.com/bstocker/gameshell.git && cd gameshell
```

**Étape 4** — Extraire l'archive :

```bash
tar -xvf GameShell.tgz
```

**Étape 5** — Appliquer le correctif de la mission 17 :

```bash
echo "true" > ./GameShell/missions/17_bg/check.sh
```

**Étape 6** — Démarrer le jeu :

```bash
./GameShell/start.sh
```

**Étape 7** — Redémarrer avec le bon encodage :

```bash
PYTHONIOENCODING=utf-8 LC_ALL=C.UTF-8 gash restart
```

---

## 🎮 Comment jouer

Lorsque vous voyez apparaître `#Mission[1]`, utilisez les commandes suivantes :

| Commande     | Rôle                                        |
|--------------|---------------------------------------------|
| `gash show`  | Découvrir l'objectif de votre mission       |
| `gash check` | Demander la validation de votre mission     |

---

## 💡 Solutions pour quelques missions difficiles

<details>
<summary><strong>Mission 3</strong></summary>

```bash
cd
cd Chateau/Batiment_principal/Salle_du_trone/
gash check
```

</details>

<details>
<summary><strong>Mission 17</strong></summary>

```bash
gash check
```

</details>

<details>
<summary><strong>Mission 18</strong></summary>

Utilisez la commande :

```bash
tree
```

</details>
