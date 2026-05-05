# Portfolio — Inès & Roksana

Site portfolio statique pour le duo de designers Inès & Roksana, inspiré de l'esthétique éditoriale sombre et minimaliste du template Nyro Silvan.

## Structure

```
/
├── index.html              → Page d'accueil (hero, à propos, projets, témoignages, footer)
├── cv.html                 → Page CV avec onglets Inès / Roksana
├── projet-erasmus.html     → Étude de cas complète — Erasmus Life
├── assets/
│   ├── css/
│   │   └── custom.css      → Styles personnalisés (Bootstrap overrides + animations)
│   └── img/                → Dossier images (à compléter)
└── README.md
```

## Stack technique

- **HTML5** sémantique
- **CSS3** avec animations keyframes pures
- **Bootstrap 5.3** via CDN
- **Bootstrap Icons** via CDN
- **Google Fonts** : Instrument Sans
- **JavaScript minimal** : scroll nav + mobile menu toggle uniquement

## Lancement

### Option 1 — Ouverture directe (simple)
```bash
open index.html
```

### Option 2 — Serveur local (recommandé pour les animations CSS)
```bash
# Python 3
python3 -m http.server 8080
# puis ouvrir http://localhost:8080

# Node.js (si installé)
npx serve .
# puis ouvrir l'URL affichée
```

## Pages

| Page | Description |
|------|-------------|
| `index.html` | Accueil avec hero animé, section à propos, projets featured et témoignages |
| `cv.html` | CV tabulaire pour Inès (UX/UI) et Roksana (Graphique & Motion) |
| `projet-erasmus.html` | Étude de cas — application mobile Erasmus Life |

## Fonctionnalités

- Gradient blob animé en CSS (rotation + scale, 22s)
- Hero text fade-up en cascade par mot
- Images flottantes avec rotation aléatoire
- Scroll reveal via `animation-timeline: view()` + fallback IntersectionObserver
- Navigation avec effet glassmorphism au scroll
- Menu mobile fullscreen
- Cards projets avec hover overlay et texte géant en arrière-plan
- Témoignages légèrement inclinés sur fond noir
- Design system SVG en guise de placeholders d'images
- Responsive mobile-first (Bootstrap breakpoints)
- `prefers-reduced-motion` respecté
