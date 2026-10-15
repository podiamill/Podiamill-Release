# Podiamill — distribution

Ce dépôt ne contient **aucun code source**. Il sert uniquement à publier les **installateurs
Windows de Podiamill**, que l'application interroge aussi pour trouver ses mises à jour.

Podiamill est un logiciel métier pour podologues : placement de gabarits de semelles et de
corrections orthopédiques sur une planche, puis découpe sur machine CNC.

## Télécharger

Les versions publiées sont dans l'onglet **[Releases](../../releases)**. Chaque release contient :

| Fichier | À quoi il sert |
|---|---|
| `Podiamill-Setup.exe` | L'installateur — **c'est le seul fichier à télécharger pour installer** |
| `Podiamill-Setup.exe.sha256` | Sa somme SHA-256, que l'application vérifie avant d'installer une mise à jour |

## Vérifier le fichier téléchargé

Chaque version publie sa **somme SHA-256** à côté de l'installateur et sur la page
« Téléchargement » du site. Pour la comparer, dans une invite de commandes Windows :

```
certutil -hashfile Podiamill-Setup.exe SHA256
```

Si les deux sommes ne correspondent pas, ne pas installer le fichier.

## Signalement d'un problème

Le suivi se fait auprès du support de Podiamill, pas dans ce dépôt.
