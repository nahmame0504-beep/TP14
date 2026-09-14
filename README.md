TP 14 - Exercice 1 : Architecture N-Tiers et Pattern DAO Générique

##  Objectifs Pédagogiques
- Mettre en œuvre une **architecture en couches (N-Tiers)** : Modèle (Bean), Persistance (DAO), Métier (Service) et Présentation.
- Concevoir un **DAO générique (`Dao<T>`)** restreint aux classes implémentant l'interface `Identifiable`.
- Créer une implémentation générique en mémoire (`ListDao<T>`) basée sur la collection `ArrayList`.
- Séparer la logique d'accès aux données des règles métiers grâce à l'injection de services (`ProfileService`, `UserService`).
- Assurer l'encapsulation et la cohérence de l'identifiant (`id`) auto-incrémenté au niveau des entités.

---


## Structure du Projet

```text
src/
└── ma/
    └── projet/
        ├── bean/
        │   ├── Identifiable.java
        │   ├── Profile.java
        │   └── Utilisateur.java
        ├── dao/
        │   ├── Dao.java
        │   └── ListDao.java
        ├── service/
        │   ├── ProfileService.java
        │   └── UserService.java
        └── TestApp.java
```
 <img width="1346" height="327" alt="EX1tp14" src="https://github.com/user-attachments/assets/fdaa3f73-d815-4d7f-a718-429b08669250" />
