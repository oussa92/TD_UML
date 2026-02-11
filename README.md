# TD UML / Reverse Engineering — Ride Sharing (type Uber)

## Contexte
Vous êtes développeur et vous rejoignez une équipe qui maintient un code existant.  
Le développeur qui a écrit ce code a quitté l’entreprise et la documentation est insuffisante.  
Votre Tech Lead vous demande de **comprendre** le projet et de **l’expliquer** à l’équipe.

La seule information métier disponible : il s’agit d’un système de ride-sharing similaire à Uber.

---

## Objectifs du TD
1. Prendre en main un projet existant (clonage, environnement, exécution).
2. Comprendre l’architecture et les concepts de conception.
3. Produire un **diagramme de classes UML** à partir du code (reverse engineering).

---

## Pré-requis
- Git
- Python 3.x
- VS Code
- draw.io (desktop ou extension VS Code)

---

## Partie 1 — Mise en place et exécution du code

### 1) Cloner le dépôt
- Ouvrir VS Code
- Ouvrir un terminal intégré
- Cloner le dépôt du projet puis se placer dans le dossier :
  - `TD_diagramme_de_classe`

### 2) Créer et activer un environnement virtuel (venv)
Créer un environnement `env`, l’activer, puis vérifier la version Python.

### 3) Lancer la démo
Exécuter le script :
- `ride_sharing_demo.py`

### 4) Résultat attendu
Après avoir lancé `ride_sharing_demo.py`, on obtient par exemple la sortie suivante :

```text
Trip 1ee5a334-3c82-4f8f-a6f2-4a7236e53600 status: IN_PROGRESS.
--------------------------------

--- Trip 1ee5a334-3c82-4f8f-a6f2-4a7236e53600 is ending ---
--- Notification for Driver Charlie ---
Trip 1ee5a334-3c82-4f8f-a6f2-4a7236e53600 status: COMPLETED.
--------------------------------

Driver Charlie is now ONLINE
Driver Charlie is now back online at Location(8.0, 8.0)

---
```
## Partie 2 — Production du diagramme UML (reverse engineering)

### Outil
Installez et utilisez **draw.io** (ou StarUML / PlantUML, au choix).

### Travail demandé
À partir du code Python fourni , produire un **diagramme de classes UML** qui contient :

1. **Classes**  
   - Inclure les classes principales du domaine et les classes “techniques”.
   - Indiquer les **attributs** pertinents.
   - Indiquer au minimum les **méthodes publiques métier**.



2. **Héritage / Interfaces / Abstractions**
   - Identifier les abstractions (ex. `ABC`, `Protocol`, classes de base).
   - Représenter les relations de généralisation / réalisation.

4. **Enumérations**
   - Lister et relier les enums utilisées (statuts, types, etc.).

5. **Patterns de conception**
   Sur le diagramme, ajouter des stéréotypes ou notes indiquant où se trouvent :
   - **Singleton**
   - **Strategy**
   - **Builder**
   - **State**
   - **Observer**

---

## Livrables
1. **1 diagramme de classes UML** (format draw.io).
2. **Une présentation courte (3 à 5 minutes)** comprenant :
   - le rôle global du système,
   - les classes principales et leurs responsabilités,
   - les relations importantes (multiplicités, composition vs association),
   - au moins 2 pistes d’amélioration.


---
