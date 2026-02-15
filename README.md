# Extension Gemini CLI : git-commit

Cette extension pour le Gemini CLI automatise la création de messages de commit en suivant la convention [Angular](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#-git-commit-guidelines).

## Fonctionnalités

- **Analyse automatique** : Analyse le `diff` des fichiers modifiés pour comprendre les changements.
- **Conformité Angular** : Génère des messages au format `<type>(<scope>): <description>`.
- **Automatisation Git** : Exécute automatiquement `git add` et `git commit` pour vous.
- **Gestion intelligente** : Capable de séparer les changements en plusieurs commits si nécessaire.

## Installation

### Installation locale

Si vous avez cloné ce dépôt, vous pouvez installer l'extension localement :

```bash
gemini extension install --local .
```

### Installation depuis GitHub

Vous pouvez installer l'extension directement depuis le dépôt distant :

```bash
gemini extension install github:q-sw/git-commit
```

## Utilisation

Une fois installée, vous pouvez utiliser la commande suivante dans n'importe quel dépôt Git :

```bash
/git-commit
```

L'assistant analysera vos changements non commités, vous proposera un message
et effectuera le commit si vous validez (ou automatiquement selon sa configuration).

## Structure des fichiers

- `gemini-extension.json` : Fichier de configuration de l'extension.
- `commands/git-commit.toml` : Définition de la commande et du prompt de l'agent.
- `GEMINI.md` : (Optionnel) Fichier de contexte spécifique pour l'extension.
