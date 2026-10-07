# Vehicle Routing Optimization (CVRP/VRPTW) — Operational Research

## Présentation
Ce projet d'Algorithmique Avancée vise à résoudre le Problème de Tournées de Véhicules (VRP / CVRP) sur des réseaux routiers de grande taille (plus de 1 000 clients). Développé dans le cadre d'un appel à projets ADEME sur la mobilité durable, le solver minimise la durée totale de parcours et les émissions de CO2 en optimisant la répartition des livraisons.

## Modélisation & Contraintes
Le modèle intègre la version de base du problème ainsi que des contraintes métier avancées :
- **Fenêtres temporelles (VRPTW) :** Respect des plages horaires de livraison et gestion des temps d'attente sur site.
- **Trafic dynamique :** Variation des temps de parcours selon les créneaux horaires.
- **Flotte hétérogène :** Gestion des capacités et des contraintes d'emprise au sol des véhicules.

## Approche Algorithmique & Performance
- **Méthode :** Conception et implémentation d'une métaheuristique (Recuit Simulé / Recherche Tabou / ALNS) en Python.
- **Benchmark & Validation :** Évaluation des performances et calcul de l'écart à l'optimal (Gap %) via l'API `vrplib` sur des instances de référence (A-n32-k5, X-n101-k25, M-n200-k17).
- **Analyse Statistique :** Génération de courbes de convergence et d'analyses de variabilité sur des séries de 20 exécutions par instance.

## Stack Technique
- **Langage :** Python (respect des normes PEP 8)
- **Bibliothèques :** `vrplib`, `numpy`, `matplotlib`, `pandas`, `jupyter`
- **Livrable :** Jupyter Notebooks d'expérimentation et scripts de résolution
