# Notes de portage — mistral-skills-mattpocock

Date du portage : 24 novembre 2026. Source : https://github.com/mattpocock/skills (branche main).

## Adaptations effectuées

- Frontmatter `SKILL.md` conservé (Agent Skills standard) et validé : `name` en slug kebab-case, `description` <= 1024 caractères.
- Les 39 skills des catégories amont (engineering, productivity, misc, deprecated, in-progress) sont toutes portées, y compris celles marquées `deprecated` ou `in-progress` dans le dépôt source.
- `disable-model-invocation` est conservé : champ supporté par Vibe (la skill reste invoquable via `/nom` mais ne se charge pas d'elle-même).

## Éléments non portés automatiquement

- Hooks et événements de session spécifiques au harnais Claude Code.
- Manifestes de marketplace (`/plugin marketplace add ...`) : Vibe Code découvre les plugins autrement (dossier `~/.vibe/plugins/` + `plugin.json`).

## Licence du contenu source

MIT (fichier LICENSE repris du dépôt d'origine)
