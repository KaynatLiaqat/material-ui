# Versions de Materiel-UI

<p class="description">Vous pouvez revenir à cette page et changer de version de document à tout moment.</p>

## Versions stables

La version la plus récente est recommandée en production.

{{"demo": "pages/versions/StableVersions.js", "hideHeader": true}}

## Versions les plus récentes

Ici vous pouvez trouver la dernière documentation non publiée et le code. Vous pouvez l'utiliser pour voir les modifications à venir et fournir des retours aux contributeurs de Material-UI.

{{"demo": "pages/versions/LatestVersions.js", "hideHeader": true}}

## Stratégie de gestion des versions

Stability ensures that reusable components and libraries, tutorials, tools, and learned practices don't become obsolete unexpectedly. Stability is essential for the ecosystem around Material-UI to thrive.

This document contains the practices that are followed to provide you with a leading-edge UI library, balanced with stability, ensuring that future changes are always introduced in a predictable way.

Matériel-UI suit strictement [la gestion sémantique des versions 2.0.0](https://semver.org/). Les numéros de version Material-UI ont trois parties : `majeur.mineur.correctifs`. Le numéro de version est incrémenté en fonction du niveau de changement inclus dans la version.

- Les ** Versions majeures ** contiennent de nouvelles fonctionnalités significatives, mais une aide minimale aux développeurs est attendue durant la mise à jour. Lors de la mise à jour vers une nouvelle version majeure, vous devrez peut-être exécuter des scripts de mise à jour, de la refactorisation du code, exécuter des tests supplémentaires et apprendre de nouvelles API.
- Les ** Versions mineures ** contiennent d'importantes nouvelles fonctionnalités. Les versions mineures sont entièrement compatibles avec les versions antérieures. aucune aide aux développeurs n'est attendue lors de la mise à jour, mais vous pouvez éventuellement modifier vos applications et vos bibliothèques pour commencer à utiliser les nouvelles API, fonctionnalités et capacités ajoutées dans la version.
- Les ** Versions de correctifs ** sont à faible risque, contiennent des corrections de bugs et de petites nouvelles fonctionnalités. Aucune assistance pour les développeurs n'est attendue lors de la mise à jour.

## Fréquence de version

A regular schedule of releases helps you plan and coordinate your updates with the continuing evolution of Material-UI.

In general, you can expect the following release cycle:

- A **major** release every 6-12 months.
- 1-3 **mineur** versions pour chaque version majeure.
- A **patch** release every week (anytime for urgent bugfix).

## Calendrier de version

> Disclaimer: The dates are offered as general guidance and may be adjusted by us when necessary to ensure delivery of a high-quality code.

| Date       | Version                    |
|:---------- |:-------------------------- |
| May 2018 ✅ | `@material-ui/core` v1.0.0 |
| May 2019 ✅ | `@material-ui/core` v4.0.0 |
| ? ⏳        | `@material-ui/core` v5.0.0 |


You can follow the [milestones](https://github.com/mui-org/material-ui/milestones) for a more detailed overview.

## Politique de support

Only the latest version of Material-UI is supported. We don't yet have the resources to offer [LTS](https://en.wikipedia.org/wiki/Long-term_support) releases.

## Pratiques de l'obsolescence

Sometimes **"breaking changes"**, such as the removal of support for select APIs and features, are necessary.

To make these transitions as easy as possible:

- The number of breaking changes is minimized, and migration tools provided when possible.
- The deprecation policy described below is followed, so that you have time to update your apps to the latest APIs and best practices.

### Deprecation policy

- Deprecated features iare announced n the changelog, and when possible, with warnings at runtime.
- When a deprecation is announced, recommended update path is provided.
- Existing use of a stable API during the deprecation period is supported, so your code will keep working during that period.
- Peer dependency updates (React) that require changes to your apps are only made in a major release.