# Convention de nommage — Festival Résonances

## Principes généraux

- Méthode : BEM.
- Langue retenue pour les classes : anglais.
- Aucun sélecteur `#id` pour le style.
- Les classes de style ne sont pas utilisées par JavaScript : le JavaScript ciblera des attributs `data-*`.
- Préfixe des composants : `c-`.
- Préfixe de mise en page : `l-`.
- Préfixe d'état : `is-`.
- Préfixe de thème : `t-`.

## Syntaxe BEM

- Bloc : `.c-button`
- Élément : `.c-card__title`
- Modificateur : `.c-button--primary`
- État : `.is-active`
- Thème : `.t-lake`, `.t-forest`, `.t-kiosk`

## Blocs de mise en page

| Bloc | Rôle |
|---|---|
| `l-container` | Conteneur principal centré |
| `l-header` | En-tête général du site |
| `l-footer` | Pied de page général |
| `l-grid` | Grille générique |
| `l-program-grid` | Organisation de la grille du programme |

Ces blocs appartiennent à `layout/` et non à `modules/`.

## Inventaire des composants

| Bloc BEM | Pages concernées | Éléments possibles | Variantes / états repérés |
|---|---|---|---|
| `c-button` | Accueil, Programme, Artiste, Billetterie, Infos | `__icon`, `__label` | `--primary`, `--secondary`, `--ghost`, `is-disabled` |
| `c-badge` | Accueil, Programme, Artiste | `__label` | `--lake`, `--forest`, `--kiosk` |
| `c-hero` | Accueil et pages internes | `__content`, `__title`, `__text`, `__actions` | `--home`, `--page` |
| `c-artist-card` | Accueil, Programme, Artiste | `__image`, `__body`, `__name`, `__meta` | `--featured`, `--compact` |
| `c-concert-card` | Programme, Artiste | `__time`, `__artist`, `__scene`, `__day` | `--lake`, `--forest`, `--kiosk` |
| `c-scene-card` | Accueil, Programme | `__title`, `__text`, `__link` | `--lake`, `--forest`, `--kiosk` |
| `c-pass-card` | Billetterie | `__title`, `__price`, `__features`, `__action` | trois formules de pass, `--featured` |
| `c-field` | Billetterie | `__label`, `__control`, `__message` | `is-error`, `is-valid`, `is-disabled` |
| `c-filter` | Programme | `__label`, `__option` | par jour, par scène, `is-active` |
| `c-faq` | Infos pratiques | `__question`, `__answer`, `__icon` | `is-open` |
| `c-info-card` | Infos pratiques | `__icon`, `__title`, `__text` | accès, horaires, services |
| `c-section-heading` | Toutes les pages | `__eyebrow`, `__title`, `__text` | `--centered` |

## Rappel

Les noms peuvent évoluer pendant le projet, mais ce fichier doit être tenu à jour à chaque étape.
