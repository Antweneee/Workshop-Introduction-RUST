# Workshop-Introduction-RUST 🦀
The goal of this project is to introduce you to the RUST programming language

## Prérequis 📝

-   Avoir Rust installé sur votre ordinateur : [https://www.rust-lang.org/learn/get-started](https://www.rust-lang.org/learn/get-started)
-   Avoir une connaissance de base de programmation

## Etape 1 : Introduction à Cargo 1️⃣

Cargo est le gestionnaire de paquet officiel de Rust. Il vous permet de gérer les dépendances de votre projet, de construire votre projet et de le publier.

Pour créer un nouveau projet avec Cargo, utilisez la commande suivante :

`cargo new mon_projet`

Cela créera un nouveau répertoire nommé "mon_projet" avec un fichier `Cargo.toml` qui décrit les dépendances de votre projet et un fichier `src/main.rs` qui contient le code source de votre projet.

Pour construire votre projet, utilisez la commande suivante :

`cargo build`

Pour exécuter votre projet, utilisez la commande suivante :

`cargo run`

## Etape 2 : Introduction au langage Rust 2️⃣

Rust est un langage de programmation de système à faible mémoire qui se concentre sur la sécurité, la performance et la concurrence. Il est conçu pour être sûr à 100% et éviter les erreurs courantes telles que les fuites mémoire et les accès à des zones mémoire non valides.

Rust possède un système de types fort et un système de propriétés de prêt qui garantissent que vous ne pouvez pas emprunter des ressources plus longtemps que nécessaire. Cela permet d'éviter les conflits d'accès à la mémoire et les erreurs courantes dans les programmes concurrents.

Pour en savoir plus sur le langage Rust, je vous invite à lire la documentation officielle : [https://doc.rust-lang.org/book/](https://doc.rust-lang.org/book/)

## Etape 3 : Exercices 3️⃣

- Ecrire un programme qui affiche "Hello World!" à l'écran.
- Demander à l'utilisateur de saisir deux nombres, puis afficher leur somme.
- Déclarer un tableau de 5 entiers et initialiser chacun d'eux avec une valeur saisie par l'utilisateur. Afficher le contenu du tableau à l'écran.
- Ecrire une fonction qui prend un nombre entier en entrée et renvoie sa factorielle (ex: 5! = 54321). Utiliser cette fonction pour calculer la factorielle d'un nombre saisi par l'utilisateur.
- Créer une structure "Personne" qui contient les champs "nom", "âge" et "adresse". Demander à l'utilisateur de saisir des informations pour 3 personnes différentes, les stocker dans des variables de type "Personne" et les afficher à l'écran.

## Etape 4 : Appel d'API 4️⃣

Dans cette étape, nous allons utiliser un bibliothèque Rust pour appeler une API. Nous allons utiliser la bibliothèque `reqwest` pour effectuer des requêtes HTTP.

Ajoutez `reqwest = "0.10"` à votre fichier `Cargo.toml` pour ajouter reqwest comme dépendance

`[dependencies] reqwest = "0.10"`

Ensuite, dans votre fichier `src/main.rs`, utilisez la bibliothèque pour effectuer une requête GET à une API :

`use reqwest::Client;  fn main() {     let client`

## Etape 5 : Mini project 5️⃣

- **1: Ajout des bibliothèques nécessaires**
    - Utiliser la bibliothèque "reqwest" pour effectuer des requêtes. HTTP pour récupérer les taux de change à partir d'une API en ligne.
    - Ajouter ces bibliothèques dans le fichier "Cargo.toml".

- **2: Ecriture du code**
    - Demander à l'utilisateur de saisir la somme d'argent, la devise d'origine et la devise de destination.
    - Utiliser la bibliothèque **"reqwest"** pour effectuer une requête HTTP à une API de taux de change pour récupérer le taux de change entre les deux devises.
    - Appliquer le taux de change à la somme d'argent pour calculer la somme convertie.
    - Afficher le résultat à l'utilisateur.

- **3: Test et déploiement**
    - Utiliser la commande "cargo run" pour exécuter votre programme et vérifier qu'il fonctionne correctement.
    - Si tout est en ordre, vous pouvez maintenant partager votre programme avec d'autres personnes ou le déployer sur un serveur.

***Note: Le taux de change peut varier au cours du temps, il est donc préférable d'utiliser une API de taux de change en temps réel pour des résultats précis.***