---
layout: page
title: Astuces
---

Redéfinir la fonte avec un peu de CSS

Comment forcer la redéfinition de la fonte avec du CSS?

Voici comment faire pour appliquer Courier / monospace:

Dans Settings > Site > Code, ajouter un script avec les options suivantes:

- Placement : End of Head.
- Page: All
- Run: On every page visit.

Contenu du code:

```html
<style>
* {
  --framer-font-family: "Courier", monospace !important;
}
</style>
```

Idem, pour utiliser Helvetica (la police système):

```html
<style>
* {
  --framer-font-family: "Helvetica Neue", "Helvetica", sans-serif !important;
}
</style>
```

Une autre option, pour avoir Helvetica, serait d'uploader "[Tex Gyre Heros](https://open-foundry.com/fonts/tex-gyre-heros)", un clone open-source.

Quelle différence entre "Helvetica Neue" et "Helvetica"? Helvetica Neue: Copyright (c) 1988, 1990, 1993 Adobe Systems Incorporated. All Rights Reserved. Helvetica: © 1990-2006 Apple Computer Inc. © 1981 Linotype AG © 1990-91 Type Solutions Inc.

## Limiter et centrer le contenu

Pour limiter le contenu (p.ex. à 1440px) et le centrer, voici un autre style CSS à appliquer:

```html
<style>
#main {
    max-width: 1440px;
    margin-left: auto;
    margin-right: auto;
}
</style>
```