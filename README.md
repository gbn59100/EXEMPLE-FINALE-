# Casa Luna – site restaurant

| Fichier | Rôle |
|---|---|
| `index.html` | Structure de la page (+ formulaire de réservation Netlify) |
| `merci.html` | Page affichée après l'envoi du formulaire |
| `css/style.css` | Design |
| `js/main.js` | Lit `content/site.json` et construit la page |
| `content/site.json` | **Tout le contenu** (textes, carte, photos, horaires…) |
| `images/uploads/` | Photos envoyées depuis l'admin |
| `admin/index.html` | Charge Decap CMS (page `/admin`) |
| `admin/config.yml` | Champs modifiables (aucun obligatoire) |
| `admin/preview.js` | Vue en direct dans l'admin |

## Mise en ligne
1. Push sur GitHub (branche `main`)
2. Netlify → Import from Git (pas de build command, publish directory = `/`)
3. Netlify → Identity → Enable (Registration : Invite only) → Services → Git Gateway → Enable
4. Identity → Invite users → email du responsable
5. Le responsable accepte l'invitation puis va sur `tonsite.netlify.app/admin`
6. Les demandes de réservation arrivent dans Netlify → Forms
