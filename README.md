# Application de gestion de l'inscription et de la réinscription en doctorat

Application web de gestion du cycle doctoral : inscription des candidats, suivi des candidatures et réinscription annuelle des doctorants, avec un parcours entièrement en ligne.

> **Statut : phase de conception.** Le dépôt contient pour l'instant la modélisation UML (diagrammes d'activité). Le code viendra dans les étapes suivantes.

## Contexte

Dans une université, l'inscription en doctorat et la réinscription annuelle passent par plusieurs acteurs (candidat, encadrant, direction de structure, centre d'études doctorales, administration) et mélangent des étapes en ligne et des étapes papier. Ce projet vise à modéliser puis à construire une application qui regroupe ce parcours dans un seul outil, avec des statuts clairs et des notifications à chaque étape.

Le projet s'inspire du fonctionnement d'une plateforme de gestion du cycle doctoral existante. Il n'est lié à aucun établissement et ne reprend aucun document interne.

## Objectifs

- Remplacer les échanges de documents papier par des téléversements et des signatures électroniques.
- Donner à chaque acteur une vue claire de ce qu'il doit faire et de l'état du dossier.
- Notifier automatiquement le candidat ou le doctorant à chaque changement de statut.
- Garder une trace de chaque décision (admission, avis du comité, validation).

## Acteurs

| Acteur | Rôle dans l'application |
|---|---|
| Candidat / doctorant | Crée son compte, choisit un sujet, dépose son dossier, remplit son rapport annuel |
| Encadrant (directeur de thèse) | Propose des sujets, examine les candidatures, signe et confirme les réinscriptions |
| Directeur de structure | Valide les sujets et les réinscriptions de sa structure |
| Centre d'études doctorales (CED) | Valide les sujets et confirme les réinscriptions |
| Administration | Vérifie les dossiers, valide les inscriptions, délivre la carte |

## Fonctionnalités prévues (version 1)

**Inscription**
- Création de compte avec activation par email
- Catalogue de sujets proposés par les encadrants
- Candidature, entretien et décision (admis, refusé, liste d'attente)
- Téléversement des documents et vérification du dossier
- Validation de l'inscription et carte numérique

**Réinscription**
- Rapport d'activités rempli en ligne, avec génération d'un PDF
- Avis du comité de suivi saisi en ligne
- Gestion des demandes de dérogation (années supplémentaires)
- Confirmations successives (directeur de thèse, structure, CED)
- Statuts visibles : en attente, validé, refusé

## Modélisation UML (début)

La modélisation commence par les diagrammes d'activité des deux parcours principaux. Les couloirs correspondent aux acteurs.


## Feuille de route

- [x] Analyse du processus d'inscription et de réinscription
- [x] Diagrammes d'activité (inscription, réinscription)
- [ ] Autres diagrammes UML (cas d'utilisation, classes, séquence, états)
- [ ] Choix des technologies et de l'architecture
- [ ] Maquettes des écrans
- [ ] Base de données et authentification
- [ ] Module inscription
- [ ] Module réinscription
- [ ] Tests et déploiement

## Structure du dépôt

```text
.
├── README.md
├── LICENSE
├── docs/
│   ├── uml/
│   │   ├── activite-inscription.md
│   │   └── activite-reinscription.md
│   └── processus.md
└── src/            (à venir)
```

## Contribuer

Le projet est en phase de conception. Les suggestions sur les diagrammes et le périmètre sont les bienvenues : ouvrir une *issue* en décrivant la proposition.

## Auteur

Mohamed Amine Sibari
