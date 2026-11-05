# UPS Workbench : versions publiées

Ce dépôt ne contient que les fichiers de **distribution** du moteur local de l'UPS Workbench
(archives de versions, empreintes sha256 et script d'installation `ups.ps1`).

Il ne contient aucune donnée clinique : ni tableaux de patients, ni jeux de données source
ou annotés. Les données de recherche ne sont publiées qu'après décision distincte.

## Installation (Windows 11, sans droits administrateur)

Dans PowerShell (console normale) :

    curl.exe -fsSL -o "$env:TEMP\ups.ps1" https://github.com/SK-Nan/UPS-Workbench-Releases/releases/latest/download/ups.ps1
    powershell -NoProfile -ExecutionPolicy Bypass -File "$env:TEMP\ups.ps1" installer

Le raccourci « UPS Workbench » est créé sur le bureau. Les clés API facultatives se placent
dans `%USERPROFILE%\UPS-Workbench\.env`.

## Versions

Voir l'onglet *Releases*. Chaque archive est accompagnée de son empreinte sha256 ; l'installateur
la vérifie avant toute installation.
