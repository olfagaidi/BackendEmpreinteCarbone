# EmpreintCarboneBackend

Ce projet représente la partie backend du module de calcul de l'empreinte carbone intégré à la solution **TraLIS ERP**. Il a été développé en **.NET** dans le cadre d'un projet de fin d'études (PFE).

## 🎯 Objectif

Permettre aux entreprises de mesurer et de visualiser leur empreinte carbone (Scope 1 et 2), à travers la collecte de données (transport, énergie, emballages, etc.), le calcul automatisé des émissions, et la génération de rapports.

## 🛠️ Technologies utilisées

- **Langage** : C# (.NET 7 ou 8)
- **Framework** : ASP.NET Core Web API
- **ORM** : Entity Framework Core
- **Base de données** : SQL Server
- **Architecture** : Monolithique
- **Outils** : Swagger, Git, Visual Studio

## 📁 Structure du projet

EmpreintCarboneBackend/
├── EmpreintCarbone/                 # API principale (.NET)
├── EmpreintCarbone.Application/    # Logique métier (services, interfaces)
├── EmpreintCarbone.Domain/         # Entités métiers (models, enums)
├── EmpreintCarbone.Infrastructure/ # Accès aux données (EF Core, repositories)
├── EmpreintCarboneProject.sln      # Solution Visual Studio
└── README.md
