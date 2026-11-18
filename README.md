# Gestion des cliniques et hôpitaux

Mini-projet de programmation orientée objet en **C#** : planification des lits, gestion des médicaments et des équipements.

## Technologies
- C# / .NET 8
- Entity Framework Core 8 (approche **Code First**)
- SQLite (`GestionHopital/hopital.db`)

## Lancer le projet
```bash
git clone <URL_DU_DEPOT>
cd <nom-du-depot>
dotnet run --project GestionHopital
```
La base est créée/mise à jour automatiquement au démarrage grâce aux migrations.

## Fonctionnalités (CRUD)
- Patients : lister, ajouter, modifier, supprimer
- Lits : lister, ajouter, changer l'état, supprimer
- Admissions : admettre, enregistrer une sortie (le lit est libéré)
- Médicaments : CRUD, retrait de stock, alertes de rupture/péremption
- Équipements : CRUD, planification et clôture des maintenances

## Migrations (rappel)
```bash
dotnet tool install --global dotnet-ef
dotnet ef migrations add NomMigration --project GestionHopital
dotnet ef database update --project GestionHopital
```

## Diagrammes
Les diagrammes UML (cas d'utilisation et classes) se trouvent dans le dossier `docs/`.

## Auteurs
[Nom Prénom] – [Nom Prénom]
