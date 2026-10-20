# Catalogue public de carrieres

Depot de DONNEES publiques (BLS / O*NET), mis a jour automatiquement par le
pipeline de donnees. Ce depot ne contient AUCUN code applicatif.

Contenu :
- `catalog/v1/careers.json` : profils de carrieres (octets faisant foi)
- `catalog/v1/manifest.json` : version, generated_at, count, sha256
- `ATTRIBUTION.md` : attribution des sources declarees par les fiches

Derniere publication : version 6, 35 carrieres, genere le 2026-10-20T23:28:25.458Z.

Verification : le sha256 des octets UTF-8 de `careers.json` doit egaler le
champ `sha256` du manifeste. Une baisse de plus de 30 % du nombre de
carrieres est refusee par le pipeline avant publication.

Usage client : telecharger `catalog/v1/manifest.json` puis `catalog/v1/careers.json`,
verifier le sha256, puis utiliser les profils.
