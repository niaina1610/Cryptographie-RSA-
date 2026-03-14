# Cryptographie RSA

Ce projet implémente les fonctions fondamentales du cryptosystème RSA, avec une approche particulière sur la factorisation de $N$ via les nombres de Mersenne et le calcul de l'inverse modulaire.

## 📌 Fonctionnalités du Code

Le script `RSA1.ipynb` est divisé en trois phases principales :

1. **Recherche de $p$ et $q$** : Une méthode de factorisation de $N$ qui teste les nombres de Mersenne ($2^i - 1$) pour identifier les facteurs premiers.
2. **Calcul de l'Indicateur d'Euler** : Une fois $p$ et $q$ obtenus, le script calcule $\phi(n) = (p-1)(q-1)$.
3. **Inverse Modulaire (Euclide Étendu)** : Une implémentation de l'algorithme d'Euclide étendu pour trouver l'inverse d'un nombre modulo $n$, essentiel pour générer la clé privée $d$.
4. **Chiffrement/Déchiffrement** : Utilisation de l'exponentiation modulaire rapide (`pow(M, k, n)`) pour transformer le message.

## 🛠️ Utilisation

### Prérequis
Le projet utilise la bibliothèque `sympy` pour la vérification de la primalité.
```bash
pip install sympy notebook
Étapes d'exécution

    Factorisation : Entrez N pour retrouver p et q.

    Clés : Saisissez p et q pour obtenir la valeur de ϕ(n) ( F dans le code).

    Opération : Entrez le message M, l'exposant k et le module n pour obtenir le résultat chiffré ou déchiffré.
```
## 🔬 Concepts Mathématiques

    Nombres de Mersenne : Forme Mi​=2i−1.

    Algorithme d'Euclide Étendu : Résolution de l'identité de Bézout ua+nb=1.

    Exponentiation Modulaire : Calcul efficace de M^k(modn).

Auteur : Voahanginiaina Roberte RANDRIANJAFY
