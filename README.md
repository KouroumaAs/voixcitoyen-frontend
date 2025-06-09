#Application de Gestion des Résultats de Référendum
Architecture Hiérarchique
Région
└── Préfecture
    └── Commune
        └── Quartier
            └── Secteur
                └── Bureau de vote (1 à n bureaux par secteur)
Données de Base par Bureau de Vote

Inscrits : Nombre total d'électeurs inscrits
Votes OUI : Nombre de votes favorables
Votes NON : Nombre de votes défavorables
Bulletins NULS : Bulletins annulés (blancs, mal remplis, etc.)
Non-votants : Inscrits - (OUI + NON + NULS)

Calculs Automatiques

Votants : OUI + NON + NULS
Suffrages exprimés : OUI + NON (hors bulletins nuls)
Taux de participation : (Votants / Inscrits) × 100
Taux d'abstention : (Non-votants / Inscrits) × 100
% OUI : (Votes OUI / Suffrages exprimés) × 100
% NON : (Votes NON / Suffrages exprimés) × 100
% Bulletins nuls : (Bulletins nuls / Votants) × 100

Tableaux de Bord par Niveau Territorial
1. Niveau Secteur

Agrégation de tous les bureaux du secteur
Comparaison inter-bureaux du secteur

2. Niveau Quartier

Synthèse de tous les secteurs du quartier
Comparaison inter-secteurs

3. Niveau Commune

Consolidation de tous les quartiers
Comparaison inter-quartiers

4. Niveau Préfecture

Vue d'ensemble de toutes les communes
Comparaison inter-communes

5. Niveau Région

Résultats globaux de toutes les préfectures
Comparaison inter-préfectures

Indicateurs Affichés par Niveau

Participation : Inscrits, Votants, Non-votants, Taux de participation
Résultats : OUI (nombre + %), NON (nombre + %), Bulletins nuls (nombre + %)
Comparaisons : Classement des entités par participation et résultats
Évolution : Suivi temps réel de la saisie

Fonctionnalités Avancées

Contrôles de cohérence : Vérification automatique des totaux
Visualisations : Graphiques (camemberts, barres), cartes géographiques
Filtres dynamiques : Par zone, taux de participation, résultats
Rapports détaillés : Procès-verbaux automatisés par niveau
Export/Import : CSV, Excel, PDF
Temps réel : Mise à jour progressive et consolidation automatique
Audit trail : Historique des saisies et modifications

Cette structure assure une remontée complète et contrôlée des résultats du bureau de vote jusqu'au niveau régional.