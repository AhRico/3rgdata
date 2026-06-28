# 3RGData — Site institutionnel

Site web de l'**Association 3RGData** — Données, Droit & Développement.

**URL de production :** [3rgdata.fr](https://3rgdata.fr)  
**Hébergement :** GitHub Pages  
**Branche principale :** `main`

---

## Présentation

Site one-page HTML/CSS/JS pur, sans framework ni bundler. Il présente l'association 3RGData, fondée en novembre 2025 à Kani-Kéli, Mayotte (SIREN 995 148 384).

### Sections

| Ancre | Contenu |
|---|---|
| `#hero` | Accroche principale + carte des zones d'intervention |
| `#about` | Présentation de l'association, missions, identité légale |
| `#president` | Mot du Président (Karim GAU.) |
| `#services` | 6 domaines d'expertise |
| `#ia` | Offre IA & Data |
| `#juridique` | Accompagnement juridique non contentieux |
| `#territory` | Carte Leaflet des implantations |
| `#values` | 4 valeurs (Intégrité, Excellence, Ancrage local, Accessibilité) |
| `#contact` | Formulaire Formspree + coordonnées |

---

## Stack technique

- **HTML/CSS/JS** — fichier unique `index.html` (1 647 lignes)
- **Polices** — Playfair Display (titres) + DM Sans (corps) via Google Fonts
- **Carte** — Leaflet.js 1.9.4 + tuiles CartoDB Light
- **Formulaire** — Formspree (`https://formspree.io/f/mlgzebkl`)
- **Cookies/RGPD** — bannière cookie maison + modales mentions légales & confidentialité

### Palette de couleurs

| Variable | Valeur | Usage |
|---|---|---|
| `--navy` | `#0D1F3C` | Couleur principale, fonds sombres |
| `--gold` | `#B8953F` | Accents, CTA, icônes |
| `--white` | `#FFFFFF` | Fonds clairs |
| `--off` | `#F9F8F5` | Fonds légèrement teintés |
| `--muted` | `#5A6A7E` | Texte secondaire |

---

## Structure des fichiers

```
3rgdata/
├── index.html          # Page principale (tout-en-un)
├── favicon.ico
├── favicon-192.png
├── favicon-512.png     # (référencé mais absent du repo)
├── apple-touch-icon.png
├── logo-3rgdata.svg
└── CNAME               # → 3rgdata.fr
```

---

## Responsive

- **≤ 960px** : grilles 2 colonnes → 1 colonne, nav masquée
- **≤ 600px** : services et valeurs en 1 colonne, formulaire pleine largeur

---

## Déploiement

Push sur `main` → GitHub Pages publie automatiquement sur `3rgdata.fr`.

```bash
git checkout main
git push origin main
```

---

## Branches

| Branche | Rôle |
|---|---|
| `main` | Production |
