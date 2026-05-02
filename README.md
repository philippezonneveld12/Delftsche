# Delftsche — Coming Soon + SEO Journal

Eenvoudige premium coming soon site voor [delftsche.com](https://delftsche.com), uitgebreid met een SEO en GEO blogstructuur zodat de website gevonden kan worden op Google en AI zoekmachines.

## Wat doet de homepage?

- Diep Delfts blauw fullscreen achtergrond met subtiele gradient, vignette en filmkorrel
- "Delftsche" in Italiana, wit, met dunne ornament-lijntjes erboven en eronder
- Vier delicate botanische hoekornamenten geïnspireerd op klassiek Delfts blauw
- "COMING SOON" onder de merknaam
- Subtiele link naar het Journal, zodat Google de blogpagina's kan crawlen
- Volledig responsive en respecteert `prefers-reduced-motion`
- SEO verbeterd met title tag, meta description, canonical, Open Graph en structured data

## Wat zit erin?

```text
/
├── index.html
├── robots.txt
├── sitemap.xml
├── llms.txt
├── README.md
├── assets/
│   └── style.css
└── blog/
    ├── index.html
    ├── amsterdam-clothing.html
    ├── kleding-amsterdam.html
    ├── dutch-clothing-brands.html
    ├── delfts-blauw-kleding.html
    └── overige SEO blogs
```

## SEO en GEO doel

De blogstructuur is gemaakt om Delftsche vindbaar te maken op onder andere:

- `amsterdam clothing`
- `clothing amsterdam`
- `kleding amsterdam`
- `Nederlandse kledingmerken`
- `Hollandse kledingmerken`
- `Dutch clothing brands`
- `Delfts blauw kleding`
- `Delft blue clothing`
- `sustainable fashion Amsterdam`
- `cadeau uit Amsterdam`

Elke blogpagina bevat:
- eigen title tag
- meta description
- canonical URL
- Open Graph tags
- Article schema
- FAQ schema
- interne links naar gerelateerde artikelen

## Online zetten

### Optie A — GitHub Pages

1. Maak een nieuwe repo aan, bijvoorbeeld `delftsche`
2. Upload alle bestanden en folders uit deze map naar de root van de repo
3. Repo → **Settings** → **Pages**
4. Source: `main` branch
5. Folder: `/ (root)`
6. Klik **Save**
7. Custom domein: voeg een `CNAME` bestand toe met inhoud:

```text
delftsche.com
```

8. Zet bij je DNS provider:

```text
A     @     185.199.108.153
A     @     185.199.109.153
A     @     185.199.110.153
A     @     185.199.111.153
CNAME www   <jouw-username>.github.io
```

### Optie B — Vercel

1. Push deze folder naar GitHub
2. Ga naar Vercel
3. Klik **New Project**
4. Importeer de repo
5. Deploy zonder extra build settings
6. Ga naar **Settings** → **Domains**
7. Voeg `delftsche.com` en `www.delftsche.com` toe
8. Volg de DNS instructies van Vercel

## Na livegang

Controleer deze URL's:

- `https://delftsche.com/`
- `https://delftsche.com/blog/`
- `https://delftsche.com/sitemap.xml`
- `https://delftsche.com/robots.txt`
- `https://delftsche.com/llms.txt`

Daarna:

1. Open Google Search Console
2. Voeg `delftsche.com` toe als property
3. Dien deze sitemap in:

```text
https://delftsche.com/sitemap.xml
```

4. Vraag indexatie aan voor:
   - homepage
   - `/blog/`
   - `/blog/amsterdam-clothing.html`
   - `/blog/kleding-amsterdam.html`
   - `/blog/delfts-blauw-kleding.html`
   - `/blog/dutch-clothing-brands.html`

## Aanpassen

- **Homepage tekst aanpassen**: open `index.html`
- **Blog styling aanpassen**: open `assets/style.css`
- **Blog teksten aanpassen**: open de losse `.html` bestanden in `/blog/`
- **Sitemap aanpassen**: open `sitemap.xml`
- **AI context aanpassen**: open `llms.txt`

## Belangrijk

Laat de `/blog/` folder online staan. De homepage mag eruitzien als een premium coming soon pagina, maar de blogfolder zorgt ervoor dat Google en AI zoekmachines Delftsche inhoudelijk kunnen begrijpen.

De kernpositie van Delftsche:

> Hollands kledingmerk geïnspireerd op Delfts blauw. Witte essentials met botanische details.
