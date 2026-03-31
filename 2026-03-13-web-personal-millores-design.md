# Millores del web personal — Disseny
Data: 2026-03-13

## Revisió d'estat (2026-03-31)

### Fet
- Homepage actualitzada en català (`themes/sx/layouts/index.html`)
- `languageCode = "ca"` a `config.toml`
- Pàgina de recerca traduïda i ampliada (`content/recerca.md`)
- Pàgina sobre mi traduïda en català (`content/sobre-mi.md`)
- Menú amb enllaços a Sobre mi, Recerca i Formacions (`themes/sx/layouts/partials/header.html`)
- Feed RSS reparat i netejat per a lectors RSS (`layouts/_default/rss.xml`)

### Pendent real
- Crear pàgina de xerrades i tallers (`content/xerrades.md`)
- Afegir "Xerrades" al menú de navegació
- Si es vol mantenir el detall curricular previst: completar `content/sobre-mi.md` amb
	títol de tesi i desglossament cronològic de rols

## Context
Web personal de Sergi Xaudiera (sergi.xaudiera.xyz). Hugo + tema custom "sx". Desplegat a GitHub Pages.

## Objectiu
Actualitzar el web per reflectir la situació professional i acadèmica actual. Mix entre presència acadèmica i professional. Idioma: **català**.

## Feina completada (commits fets)

### Correccions (commit `3d2e105`)
- "Google Shcolar" → "Google Scholar" (`content/publications.md`)
- "Minimalismo digial" → "Minimalismo digital" (`content/reading.md`)
- Meta description moguda de hardcoded a `config.toml` `[params]`
- Eliminat meta description duplicat a `baseof.html`

---

## Opció A — Actualització de contingut (gairebé completada)

### ✅ Homepage (`themes/sx/layouts/index.html`) — APROVADA

Text nou en català:

```
Soc doctor en Societat de la Informació i el Coneixement per la Universitat Oberta de
Catalunya. La meva recerca se centra en la gestió de la desinformació i les infodèmies
en situacions d'emergència — com es difonen els missatges en canals digitals, com
afecten les persones i com podem respondre-hi.

La meva expertesa és la transformació digital: com les eines digitals connecten les
persones pel bé comú. M'agrada aplicar enfocaments innovadors per resoldre reptes
reals, i crec en adaptar les noves tecnologies per millorar la vida de les persones.

Treballo a la Generalitat de Catalunya com a responsable del desplegament de casos
d'ús d'IA a l'administració pública. També col·laboro amb Ersilia [https://ersilia.io],
una iniciativa de codi obert que aplica la IA a la recerca en salut global.
Anteriorment, vaig fundar Numballs [/numballs/], un projecte que em va ensenyar molt
sobre com extreure coneixement de les dades de xarxes socials.

Em pots trobar a Mastodon [https://mastodon.social/@sxau].
```

### ⏸️ About (`content/sobre-mi.md`) — PENDENT PARCIAL

Canvis acordats parcialment:
- Traduir tot al català
- PhD: canviar "2019 – Present" → "2019–2024"
- Afegir títol de la tesi: *La gestió de la infodèmia i la desinformació en situacions d'emergència. Una perspectiva des de Catalunya*
- Actualitzar càrrec a la Generalitat (pendent decidir si separar Digital Strategist / Responsable IA o mantenir com a càrrec evolutiu)
- Afegir Ersilia (2024–present)
- Traduir totes les seccions (Acadèmic, Experiència, Competències, Referències)

Preguntes obertes:
1. Separar Generalitat en dos registres (Digital Strategist 2010–2024 / Responsable IA 2024–present) o mantenir com un de sol?
2. Afegir noves eines a competències (Python, LLMs...)?

### ✅ Research (`content/recerca.md`) — FET
- Traduït al català
- Ampliat amb context i projectes actuals

### ⏸️ Xerrades (`content/xerrades.md`) — PENDENT (secció nova)
- Crear nova pàgina de xerrades i tallers
- Afegir al menú de navegació
- Referència d'estil: https://jorgesanz.net/talks/

### ✅ Idioma global — FET
- `config.toml`: `languageCode = "ca"`
- Impacte aplicat: atribut `lang` de l'HTML

---

## Opcions futures (B i C) — No iniciades

### Opció B — Renovació completa
- Migrar ~150 posts de blog (2007–2020) des de https://github.com/xxxaau/sergi.site/tree/master/_posts
- Crear Link Blog (estil Simon Willison)
- Etiquetes de verificació Mastodon

### Opció C — Actualització + blog progressiu (recomanada per continuar)
- Tot de l'opció A
- Importar 20–30 posts seleccionats del blog antic
- Crear estructura de Link Blog
- Etiquetes Mastodon (`rel="me"` i verificació de periodisme)

---

## Altres millores identificades (no prioritzades)

- Open Graph tags (`og:title`, `og:description`, `og:image`) — millora SEO i compartició
- Twitter/X cards
- `X-UA-Compatible IE=edge` obsolet — es pot eliminar
- Simplificar header.html (codi duplicat home/no-home)
- `sidebar.html` buit — eliminar o usar
- `languageCode` incorrecte (en-us quan el contingut és català/castellà)
